## Add maven jar to local repo

### Pattern

mvn install:install-file -Dfile=c:\kaptcha-{version}.jar -DgroupId=com.google.code
-DartifactId=kaptcha -Dversion={version} -Dpackaging=jar

### Example
```
mvn install:install-file -Dfile=d:/FMS/consoleframe/OpsPortalMgmt/Access/lib/proxool-0.9.1.jar -DgroupId=proxool -DartifactId=proxool -Dversion=0.9.1 -Dpackaging=jar

mvn install:install-file -Dfile=d:/FMS/consoleframe/OpsPortalMgmt/Access/lib/proxool-cglib.jar -DgroupId=proxool-cglib -DartifactId=proxool -Dversion=0.9.1 -Dpackaging=jar


mvn install:install-file -Dfile=d:/FMS/consoleframe/OpsPortalMgmt/Access/lib/jboss-transaction-api_1.2_spec-{version}.jar -DgroupId=org.jboss.spec.javax.transaction -DartifactId=jboss-transaction-api_1.2_spec -Dversion=1.0.0.Alpha3 -Dpackaging=jar
```

### Links
http://www.mkyong.com/maven/how-to-include-library-manully-into-maven-local-repository/
