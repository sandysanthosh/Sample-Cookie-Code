Welcome to the Sample-Cookie-Code wiki!


`protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
	response.setContentType("text/html");
	PrintWriter pw=response.getWriter();
	
	Cookie  cookie=new Cookie("url","hai");
	cookie.setMaxAge(60*60);// 1 hour 
	response.addCookie(cookie);
	pw.println("Created Cookie");
	
	
	}
`
