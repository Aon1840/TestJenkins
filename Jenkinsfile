pipeline {
    agent any

    stages {
        stage ('Checkout and Setup') {
            step {
                sh 'cd fastlane'
            }
        }

        stage ('Clean project') {
            step {
                sh 'bundle exec fastlane clean'
            }
        }

        stage ('Run Unittest') {
            steps {
                sh 'bundle exec fastlane unittest'
            }
        }

        stage ('Build') {
            steps {
                sh 'bungdle exec fastlane build'
            }
        }
    }
}