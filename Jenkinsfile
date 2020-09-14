node 
{
    
  stage('Stage mvn')
  {

    steps
      {
        sh 'mvn install'
      }
      
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
