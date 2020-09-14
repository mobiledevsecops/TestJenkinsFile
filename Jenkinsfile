

node {
  stage ('Build') {
    //git url: 'https://github.com/cyrille-leclerc/multi-module-maven-project'
    //git url: 'https://github.com/mobiledevsecops/TestJenkinsFile'
    withMaven {
      sh "mvn clean verify"
    } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
  }
}

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
