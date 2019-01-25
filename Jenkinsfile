pipeline {
    agent any
    tools {
        maven 'mvn_3.6.0'
        jdk 'jdk_8.202'
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }

        stage ('Build') {
            steps {
                sh 'mvn clean install' 
            }
            }
        }
    }

