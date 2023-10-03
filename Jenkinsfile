//CODE_CHANGES = getGitChances()
pipeline {

    agent any
    environments {
         NEW_VERSION = '1.3.0'
         SERVER_CREDENTIALS = credentials ('server-credentials')
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
        echo "deploying with ${SERVER_CREDENTIALS}"
        //withCredentials ([
         //   usernamePassword(credentials: 'server-credentials', usernameVariable: USER, passwordVariable: PWD)
        //]) {
        //sh "some script ${USER} ${PWD}"
      }
    }
  }
    //post {
     //   always {
            //
    //    }
    //    success {
            //
    //    }
    //    failture {
            //
    //    }
    //}
}
