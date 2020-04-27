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
        stage('--execute--') {
            steps {
                 sh '''#!/bin/bash
                echo "Step: Execute Hello Singam"
                '''
		sh 'hellosingam.bat'
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
