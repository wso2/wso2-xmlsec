# wso2-xmlsec
This is a fork of Apache santuario-xml-security-java repository. Forked @ tag level 1.5.6

# Patching instructions
After doing a code change build this repository with JDK 6 + maven 3.2.5 combination.
You can download JDK 6 from atuwa (internal)
We  are skipping tests in the default profile. So, to build with tests use the following command.
```
mvn clean install -P withtest
```
