pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 build job: 'PES1UG20CS483-1', wait: false
                 echo 'Successfully built -Neha'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Test -Neha'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Successfully Deployed -Neha'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
