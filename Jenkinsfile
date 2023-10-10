declarative pipeline:

pipeline{
	agent any
	stages{
		stage('1-clonecode'){
			steps{
				checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'team7-git-id', url: 'https://github.com/GalaxyApp1/TeeApp.git']])
			}
		}
		stage('2-artifactbuild'){
			steps{
				sh 'action2'
			}
		}
		stage('3-unitest'){
			steps{
				sh 'actions3'
			}
		}
	} 
}
