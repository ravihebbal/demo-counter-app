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
                sh "mvn -e -X clean test"
            }
        }

        stage('Integration testing'){

            steps{
                sh "mvn -e -X verify -DskipUnitTests"
            }
        }

    }
}
