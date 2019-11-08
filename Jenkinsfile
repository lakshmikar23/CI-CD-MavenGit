pipeline {
	agent {
              label 'Linux-leb'
              }
	stages {
		stage('---clean---'){
			steps {
				tool name: 'Maven3.6.2', type: 'maven'
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				tool name: 'Maven3.5.4', type: 'maven'
				sh "mvn test"
			}
		}
		stage('---package---'){
			steps {
				tool name: 'Maven3.3.3', type: 'maven'
				sh "mvn package"
			}
		}
	}
}
         
