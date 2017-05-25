First u have to create dsn: NetConference


to set the classpath
set classpath=C:\jakarta-tomcat-5\dist\common\lib\servlet-api.jar;%classpath%;.;

create WEB-INF folder and place web.xml file

in web.xml file write according to the classes present in the project

ex....:-

<web-app>
<servlet>
<servlet-name>ac</servlet-name>
<servlet-class>ac</servlet-class>
</servlet>
<servlet-mapping>
<servlet-name>ac</servlet-name>
<url-pattern>/ac</url-pattern>
</servlet-mapping>
</web-app>

============================

javac -d ./WEB-INF/classes *.java

jar -cvf servlet.war WEB-INF *.html

start startup.bat from C:\jakarta-tomcat-5\dist\bin

after running server........

Open InternetExplorer 

give url :-= http://localhost:8081/manager/html