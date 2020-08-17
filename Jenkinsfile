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
                nodejs(nodeJSInstallationName: 'NodeJs') {
                    sh 'npm --version'
                    sh 'npm cache clean --force'
                    sh 'npm install'
                }
            }
        }
        stage('Artifact') {
            steps {
                echo 'Building artifact'                
            }
        }
    }
}
