pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {
    
    when {
     branch "main"
      }

    stage('main branch') {

      steps {

        echo "this is main branch"

      }

    }
    stage('test branch') {

      when{
      branch "test"
      }
      steps {

        echo "this is test branch"

      }

    }
    
    stage('feature branch') {

      when{
      branch "feature"
      }
      steps {

        echo "this is feature branch"

      }

    }

  }

}
