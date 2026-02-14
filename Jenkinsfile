pipeline {
    agent any

    stages {
        stage('Get the code from GitHub') {
            steps {
                git branch: 'main', url: 'https://github.com/Vinay21211/pet_shop.git'
            }
        }

        stage('Build with Maven') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}

