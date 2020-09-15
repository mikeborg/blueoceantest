pipeline {
    agent any
    stages {
        stage('Static Analysis') {
            steps {
                echo 'Static Code Analysis..'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'make'
                sh './hello.exe'
            }
        }
        stage('Unit Test') {
            steps {
                echo 'Unit Testing...'
            }
        }
        stage('Flash') {
            steps {
                echo 'Flash Microcontroller...'
            }
        }
        stage('Blackbox') {
            steps {
                echo 'Blockbox Testing...'
            }
        }
        stage('Accept & Merge')
        {
            steps {
                echo 'Pull Request'
            }
        }
    }
}