@Library('shared-lib') _

pipeline {
    agent any

    stages {
        stage('Build via Shared Library') {
            steps {
                mavenBuild(mavenCmd: 'mvn clean package')
            }
        }
    }
}
