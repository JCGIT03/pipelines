
pipeline {
    agent any
    parameters {
        //string(name: 'VERSION', defaultValue '', description: 'version to deploy on prod')
        choice(name: 'VERSION', choices: ['1.1.0','1.2.0',1.3.0],description: '')
        booleanParam(name: 'executeTests', defaultValue: true, description: '')
    }
  stages { 
    stage("build") {
      steps {
        echo 'building the aplication...'
      }
    }
    stage("test") {
        when {
            expression {
                params.executeTests
            }
        }
       steps {
        echo 'testing the aplication...'
      }
    }
    stage("deploy") {
       steps {
        echo 'deploying the aplication...'
        echo "deploying version ${params.VERSION}"
      }
    }
  }
}
