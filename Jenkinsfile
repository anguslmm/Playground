pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                cmakeBuild
                    installation: 'InSearchPath',
                    steps: [
                        [args: 'all']
                    ]
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}