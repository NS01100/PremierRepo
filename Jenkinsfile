pipeline {
	agent any
	stages {
		stage('Clone') {
			steps {
				sh "rm -rf *"
				sh "git clone https://github.com/NS01100/PremierRepo.git"
			}
		}
		stage('Build') {
			steps {
				sh "cd PremierRepo && javac Main.java"
			}
		}
		stage('Run') {
			steps {
				sh "cd PremierRepo && java Main"
			}
		}
	}
}
