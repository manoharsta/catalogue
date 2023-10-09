pipeline {
    agent { node { label 'AGENT-1' } }
    stages {
        stage('Install depdencies') {
            steps {
                // INstalling dependencies
                sh 'npm install'
            }
        }
        stage('Unit test') {
            steps {
                //just printing
                echo "unit testing is done here"
            }
        }
        // sonar-scanner command expect sonar-project.properties should be available
        stage('Sonar Scan') {
            steps {
                sh 'ls -ltr'
                sh 'sonar-scanner'
            }
        }
    }
}

