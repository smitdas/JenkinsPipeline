pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Aniket will go to class 2'
          }
        }

        stage('Test') {
          steps {
            echo 'Anvita plays all day'
            echo '"The path is - ${ChromeDriverPath}"'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Mummy cooks food and looks after Aniket and Anvita all day'
      }
    }

  }
  environment {
    ChromeDriverPath = 'C:\\Software\\sonarqube-8.6.1.40680\\bin\\windows-x86-64'
  }
}