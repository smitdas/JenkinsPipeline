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
            echo "The path is - ${ChromeDriverPath}"
          }
        }

        stage('Test Log') {
          steps {
            writeFile(file: 'LogTestFile.txt', text: "This is an automation file: - ${ChromeDriverPath}")
          }
        }

      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            input(message: 'Do you really want to deploy?', id: 'OK')
            echo 'Mummy cooks food and looks after Aniket and Anvita all day'
          }
        }

        stage('Artifacts') {
          steps {
            archiveArtifacts 'LogTestFile.txt'
          }
        }

      }
    }

  }
  environment {
    ChromeDriverPath = 'C:\\Software\\sonarqube-8.6.1.40680\\bin\\windows-x86-64'
  }
}