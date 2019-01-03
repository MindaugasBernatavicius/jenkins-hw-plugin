# jenkins-hw-plugin

Example projects ant resources:

- THE BIBLE:
https://wiki.jenkins.io/display/JENKINS/Extend+Jenkins

- Tutorial on how to create a basic Jenkins plugin:
https://wiki.jenkins.io/display/JENKINS/Plugin+tutorial

- Example:
https://github.com/HPEbot/hello-world-plugin-2/blob/master/src/main/java/hudson/plugins/hello_world/HelloWorldBuilder.java

- An additional explanation (w/ project layout):
https://blog.codecentric.de/en/2012/08/tutorial-create-a-jenkins-plugin-to-integrate-jenkins-and-nexus-repository/

    ```
    .
    ├── pom.xml
    └── src
        └── main
            ├── java
            │   └── de
            │       └── mb
            │           └── HelloWorldBuilder.java
            └── resources
                ├── de
                │   └── mb
                │       └── HelloWorldBuilder
                │           ├── config.jelly
                │           ├── global.jelly
                │           ├── help-name.html
                │           └── help-useFrench.html
                └── index.jelly
    ```


Gotchas:
- Help tags in the.jelly markup have this generated URI: http://192.168.56.11:8080/descriptor/io.jenkins.plugins.helloWorld.HelloWorldBuilder/help/useFrench 
