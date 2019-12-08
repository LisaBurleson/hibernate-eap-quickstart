# Converted the jboss starter to gradle

1. ran `gradle init` - this will generate a build.gradle, settings.gradle, gradlew, gradlew.bat
2. modified the dependencies versions by removing the "-redhat*" suffix because they won't resolve
3. added mavenCentral() to the repositories

Finally all the dependencies resolved and were successfully added to the classpath.

# Getting started
1. before launching ide, open console to this foled and run `./gradlew.bat eclipse` or `./gradlew.bat idea`
2. import the existing project into your ide
3. create the jboss server for deployment
4. deploy/run the app and open a browswer to http://localhost:8080/hibernate-7.2.0.GA/index.jsf