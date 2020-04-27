pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                sh '''#!/bin/bash
                echo "Step: Clean"
                '''
            }
        }
        stage('--test--') {
            steps {
                 sh '''#!/bin/bash
                echo "Step: Test"
                '''
            }
        }
        stage('--package--') {
            steps {
                sh '''#!/bin/bash
                echo "Step: Package"
                '''
            }
        }
    }
}
