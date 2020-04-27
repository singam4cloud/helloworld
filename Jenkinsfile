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
        stage('--deploy--') {
            steps {
                 sh '''#!/bin/bash
                echo "Step: Deploy HelloSingam.bat"
		mkdir /opt/helloworld
		./hellosingam.bat > /opt/helloworld/hellosingam.txt
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
