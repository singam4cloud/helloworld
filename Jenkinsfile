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
		mkdir helloworld
		git clone https://github.com/singam4cloud/helloworld.git
		git checkout cisco-cr1
		./hellosingam.bat > helloworld/hellosingam.txt
		cat >> helloworld/hellosingam.txt << "EOF"
		************* Successfully executed *************
		EOF
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
