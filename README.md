


**Issue**

Failed to instantiate SLF4J LoggerFactory:

**Solution**

https://stackoverflow.com/questions/40138247/maven-spring-boot-failed-to-instantiate-slf4j-loggerfactory-reported-exception

or 

Below actions worked for me

`Run mvn dependency:purge-local-repository` to remove all dependencies and force a re-download.
Then do a `mvn clean verify`

**Issue**

The server time zone value ‘EDT’ is unrecognized or represents more than one time zone.” error appears with MySQL JDBC Driver in MicroStrategy 10.4.x and above

**Error Reason**

https://community.microstrategy.com/s/article/KB442386-The-server-time-zone-value-EDT-is-unrecognized-or-represents-more-than-one-time-zone-error-appears-with-MySQL-JDBC-Driver-in-MicroStrategy-10-4-x-and-above?language=en_US

**Solution**

https://stackoverflow.com/questions/26515700/mysql-jdbc-driver-5-1-33-time-zone-issue

jdbc:mysql://localhost/db?useUnicode=true&useJDBCCompliantTimezoneShift=true&useLegacyDatetimeCode=false&serverTimezone=UTC

or

jdbc:mysql://127.0.0.1:3306/test?serverTimezone=UTC
