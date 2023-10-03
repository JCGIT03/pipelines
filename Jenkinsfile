//CODE_CHANGES = getGitChances()
pipeline {

    agent any
     tools {
        maven 'Maven'
        
         
     }
    
  stages { 
    stage("build") {
      steps {
        echo 'building the aplication...'
        sh "mvn install"
      }
    }
    stage("test") {
       steps {
        echo 'testing the aplication...'
      }
    }
    stage("deploy") {
       steps {
        echo 'deploying the aplication...'
      }
    }
  }
}
