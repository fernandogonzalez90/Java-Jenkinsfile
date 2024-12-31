pipeline {
    agen any
    stages {
        stage('Clonando repo'){
            steps{
                git "git@github.com:fernandogonzalez90/Java-Jenkinsfile.git"
            }
        }
        stage('Construyendo Java'){
            steps{
                sh 'mvn clean install'
            }
        }
        stage('Ejecutando los test'){
            steps{
                sh 'mvn test'
            }
        }
    }
}