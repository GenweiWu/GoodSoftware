# GoodEditor
好用的idea编辑器的使用技巧

## IntelliJ IDEA使用技巧
- [调整java进行import时的顺序，跟eclipse默认的一致：](https://stackoverflow.com/a/17194980/6182927)
- [好用的编程字体](https://github.com/yakumioto/YaHei-Consolas-Hybrid-1.12)
- 规避解决无法运行springBoot war包的问题：  
  - [官方bug链接](https://youtrack.jetbrains.com/issue/IDEA-107048)  
  - 规避方法为：
  
  > I was able to make this work by changing the scope of the spring-boot-starter-tomcat dependency to compile under Project structure->Dependencies tab. This doesn't effect pom.xml but allows this dependencies to be available to spring boot run configuration  
  
  具体修改的包如下：
  ```
    Maven: org.springframework.boot:spring-boot-starter-tomcat
    Maven: org.apache.tomcat.embed:tomcat-embed-core
    Maven: org.apache.tomcat.embed:tomcat-embed-el
    Maven: org.apache.tomcat.embed:tomcat-embed-logging-juli
    Maven: org.apache.tomcat.embed:tomcat-embed-websocket
    Maven: org.apache.tomcat.embed:tomcat-embed-jasper 
  ```
   
