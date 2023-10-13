pipeline{
    agent any
    stages {
        stage('GIT checkout') {
            steps {
                git 'https://github.com/Saish40/Springboot.git'
            }
        }
        stage('Validate') {
            steps {
                sh 'mvn validate'
            }
        }
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
        stage('Install') {
            steps {
                sh 'mvn install'
            }
        }
    }
}
