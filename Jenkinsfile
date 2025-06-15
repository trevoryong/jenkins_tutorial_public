pipeline {
    agent { 
       any
      }
    triggers {
        pollSCM '*/5 * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh 'pwd'
                echo "build complete"
                
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh 'ls'
                echo "test complete"
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh 'cat /etc/os*release'
                echo "delivery complete"
                
            }
        }
    }
}