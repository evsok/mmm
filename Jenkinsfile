pipeline {
    agent {
      label "agent11-optimised"
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo '********************** Hostname:'
                sh 'hostname'
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo '********************** Hostname:'
                sh 'hostname'                
                sh 'mvn exec:java'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
