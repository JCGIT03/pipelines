//CODE_CHANGES = getGitChances()
pipeline {

    agent any
    environments {
         NEW_VERSION = '1.3.0'
         SERVER_CREDENTIALS = credentials ('')
    }
  stages { 
    stage("build") {
      steps {
        echo 'building the aplication...'
        echo "building version ${NEW_VERSION}"
      }
    }
    stage("test") {
        //when {
            //expression {
                //BRANCH_NAME == 'master' || BRANCH_NAME == 'main'
                //BRANCH_NAME == 'master' && CODE_CHANGES == true
            //}
        //}
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
    post {
        always {
            //
        }
        success {
            //
        }
        failture {
            //
        }
    }
}
