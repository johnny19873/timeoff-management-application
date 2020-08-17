pipeline {
    agent any 
    stages {
        stage('GitHub') {
            steps {
                echo 'Clonning git'
                //sh 'mvn --version'
                git url: 'https://github.com/johnny19873/timeoff-management-application.git'
            }
        }
        stage('Build npm') {
            steps {
                echo 'Build npm'
                //sh 'mvn --version'
                
            }
        }
    }
}
