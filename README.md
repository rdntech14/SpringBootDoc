## What is Micro Service?

https://www.tutorialspoint.com/spring_boot/spring_boot_introduction.htm

## What is Spring Boot?

https://www.tutorialspoint.com/spring_boot/spring_boot_introduction.htm

## Spring Boot Advantages

https://www.tutorialspoint.com/spring_boot/spring_boot_introduction.htm

* Simplified & version conflict free dependency management through the **starter POMs**. like spring-core.jar, spring-webmvc.jar, spring-web.jar, spring-boot-starter-data-jpa, Spring boot web starter.

* **Dependencies Management** - We can quickly setup and run standalone, web applications and micro services at very less time.

* You can just assemble the jar artifact which comes with an **embedded Tomact**, Jetty or Undertow application server and you are ready to go.

* Spring Boot provides HTTP endpoints to access application internals like detailed metrics, application inner working, health status, etc.

* **Annotation-Based Configuration - No XML based configurations** at all. Very much simplified properties. The beans are initialized, configured and wired automatically.

* The **Spring Initializer** provides a project generator to make you productive with the certain technology stack from the beginning. You can create a skeleton project with web, data access (relational and NoSQL datastores), cloud, or messaging support.

**Issue**

Failed to instantiate SLF4J LoggerFactory:

**Solution**

https://stackoverflow.com/questions/40138247/maven-spring-boot-failed-to-instantiate-slf4j-loggerfactory-reported-exception

or 

Below actions worked for me

`Run mvn dependency:purge-local-repository` to remove all dependencies and force a re-download.
Then do a `mvn clean verify`

**Common Issue**

The server time zone value ‘EDT’ is unrecognized or represents more than one time zone.” error appears with MySQL JDBC Driver in MicroStrategy 10.4.x and above

**Error Reason**

https://community.microstrategy.com/s/article/KB442386-The-server-time-zone-value-EDT-is-unrecognized-or-represents-more-than-one-time-zone-error-appears-with-MySQL-JDBC-Driver-in-MicroStrategy-10-4-x-and-above?language=en_US

**Solution**

https://stackoverflow.com/questions/26515700/mysql-jdbc-driver-5-1-33-time-zone-issue

`jdbc:mysql://localhost/db?useUnicode=true&useJDBCCompliantTimezoneShift=true&useLegacyDatetimeCode=false&serverTimezone=UTC`

or

`jdbc:mysql://127.0.0.1:3306/test?serverTimezone=UTC`
