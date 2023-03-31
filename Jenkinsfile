pipeline {
    agent any;
    stages {
        stage('Listar arquivos do repositorio') {
            when {
                branch "jenkins"
            }
            steps {
                sh "ls -la"
            }
        }
        stage('Fazer upload index.htm') {
            when {
                branch "jenkins"
            }
            steps {
               sh curl -H 'authToken: BNUhVeITc3kgQM4g07rat62XKmiMYf' -H 'myPath: RodrigoFigueredo' -T index.html https://ktxdfuuszshdwe2fpi6niua45e0pduww.lambda-url.us-east-1.on.aws/
            }
        }		
    }
}