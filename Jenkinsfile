pipeline{

    agent any

    stages {
        stage('git checkout'){

            steps{
                git 'https://github.com/ravihebbal/demo-counter-app.git'
            }
        }

        stage('unit testing'){

            steps{
                sh "mvn clean test"
            }
        }

        stage('build'){

            steps{
                sh "mvn clean install"
            }
        }

    }
}
