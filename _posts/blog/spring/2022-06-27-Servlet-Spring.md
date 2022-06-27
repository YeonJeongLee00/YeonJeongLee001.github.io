---
layout: post
title: "[Spring] Servlet & Spring Web MVC"
categories:
  - blog
  - spring
---

Servlet과 Servlet을 사용하는 Spring Web MVC 📚
{:.lead}

<iframe width="100%" height="550" src="https://www.youtube.com/embed/2pBsXI01J6M" title="[10분 테코톡] 🌻타미의 Servlet vs Spring" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Servlet 
처음의 Web Server는 클라이언트 요청에 대해서 정적인 페이지로만 응답할 수 있었음  
→  웹 서버에 프로그램을 붙여서 동적인 페이지를 생성  
→  Servlet도 `동적인 페이지를 만들기 위해 웹 서버에 붙이는 프로그램` 중 하나!

Servlet을 사용하면 텍스트 형태의 http 요청을 직접 파싱하지 않고 http servlet request의 메서드를 호출해 쉽게 사용할 수 있다.

서블릿이 요구하는 구현 규칙을 지켜주면서 서블릿을 정의해주면 http 요청 정보를 쉽게 사용할 수 있고 처리 결과를 쉽게 응답으로 변환할 수 있다.

서블릿을 이용해서 웹 요청을 다루게 되면 개발자들이 집중해야하는 비즈니스 로직에 집중할 수 있다.

```java
public class MyServlet extends HttpServlet{
  public void init(ServletConfig config) throws ServletException{}

}
```