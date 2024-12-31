pipeline {
    agent any
    stages {
        stage('Clonando repo'){
            steps{
                git branch: 'main', url: "https://github.com/fernandogonzalez90/Java-Jenkinsfile.git"
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