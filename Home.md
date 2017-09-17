Welcome to the Sample-Cookie-Code wiki!


`protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
	response.setContentType("text/html");
	PrintWriter pw=response.getWriter();
        String n=request.getParameter("userName");  
        out.print("Welcome "+n);  
  
        Cookie cookie=new Cookie("uname",n);//creating cookie object  
	cookie.setMaxAge(60*60);// 1 hour 
	response.addCookie(cookie);
	pw.println("Created Cookie");
	
	
	}
`
