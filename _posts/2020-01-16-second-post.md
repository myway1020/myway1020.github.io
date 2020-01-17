---
title:  "jstl특정시간에 이미지 변경하기"
excerpt: "특정시간이되면 이미지 변경을 시도한다."

categories:
  - Blog
tags:
  - Blog
last_modified_at: 2020-01-17T24:20:00-50:00
---

```jsp
    <h1>
        <a href="/main.do">
        <jsp:useBean id="now" class="java.util.Date" />
        <fmt:parseDate value="202001141331" pattern="yyyyMMddkkmm" var="endDate" />
        <fmt:formatDate value="${now}" pattern="yyyyMMddkkmm" var="nowDate" />
        <fmt:formatDate value="${endDate}" pattern="yyyyMMddkkmm" var="closeDate"/>
        <c:choose>
            <c:when test="${ closeDate > nowDate}">
            <img src="<c:url value='/{filepath}/{기존_파일명}.png'/>" alt="">
            </c:when>
            <c:otherwise>
            <img src="<c:url value='/{filepath}/{변경_파일명}.png'/>" alt="" style="margin-top: 0px;">
            </c:otherwise>
        </c:choose>
        </a>
    </h1>
```

YFM에서 정의한 제목을 이중 괄호 구문으로 본문에 추가할 수 있다.
이 글의 제목은 {{ page.title }}이고
마지막으로 수정된 시간은 {{ page.last_modified_at }}이다.
