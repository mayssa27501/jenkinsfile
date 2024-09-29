pipeline {
    agent any
    tools {
        maven 'M2_HOME'
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('GIT') {
            steps {
                git branch: 'master',
                url: 'https://github.com/hwafa/timesheetproject.git'
            }
        }
        stage('CLEAN') {
            steps {
                sh "mvn clean"
            }
        }
        stage('COMPILE') {
            steps {
                sh "mvn compile"
            }
        }
        
    }
}