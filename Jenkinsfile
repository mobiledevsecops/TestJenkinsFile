<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>com.example</groupId>
    <artifactId>demo-parent</artifactId>
    <version>0.0.30-SNAPSHOT</version>
    <packaging>pom</packaging>

    <name>demo-parent</name>
    <description>Demo multi module project</description>

    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>2.1.6.RELEASE</version>
        <relativePath />
    </parent>
    <properties>
        <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
        <project.reporting.outputEncoding>UTF-8</project.reporting.outputEncoding>
        <java.version>1.8</java.version>
       
        <project.scm.id>github.com</project.scm.id>
    </properties>
    <modules>
        <module>shared-core</module>
        <module>demo-1</module>
        <module>demo-2</module>
    </modules>
    
    <build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-release-plugin</artifactId>
                <version>2.5.3</version>
            </plugin>
        </plugins>
    </build>
    <distributionManagement>
        <snapshotRepository>
            <id>nexus3.beescloud.com</id>
            <url>https://nexus3.beescloud.com/repository/maven-snapshots/</url>
        </snapshotRepository>
        <repository>
            <id>nexus3.beescloud.com</id>
            <url>https://nexus3.beescloud.com/repository/maven-releases/</url>
        </repository>
    </distributionManagement>
</project>

/*

node {
  stage ('Build') {
    //git url: 'https://github.com/cyrille-leclerc/multi-module-maven-project'
    git url: 'https://github.com/mobiledevsecops/TestJenkinsFile'
    withMaven {
      sh "mvn clean verify"
    } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
  }
}

*/
/*

node 
{
  
  stage('Stage Checkout')
  {

    checkout scm
    sh 'git submodule update --init'  
  }

  stage('Create build output')
  {
    // Make the output directory.
    sh "mkdir -p output"

    // Write an useful file, which is needed to be archived.
    writeFile file: "output/usefulfile.txt", text: "This file is useful, need to archive it."

    // Write an useless file, which is not needed to be archived.
    writeFile file: "output/uselessfile.md", text: "This file is useless, no need to archive it."
  }
  
  stage('Maven build') 
  {
        buildInfo = rtMaven.run pom: 'maven-example/pom.xml', goals: 'clean install'
    }
  
}
  
*/
