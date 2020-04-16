pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                cmakeBuild
                    buildDir: 'build',
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