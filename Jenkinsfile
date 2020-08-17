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
                withNPM(npmrcConfig: 'd4433e47-d1b9-4716-842c-fae11bc84b13') {
                    sh 'sudo apt install nodejs'
                    //sh 'npm install'
                    //sh 'npm --version'
                }
            }
        }
    }
}
