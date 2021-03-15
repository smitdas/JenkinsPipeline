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
}