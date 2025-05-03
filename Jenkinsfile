@Library('shared-lib') _

pipeline {
    agent any

    environment {
        IMAGE_NAME = "yogeshpri/javaimgg"
        REGISTRY = "docker.io"
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build via Shared Library') {
            steps {
                mavenBuild(mavenCmd: 'mvn clean package')
            }
        }
    }
}
