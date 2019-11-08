pipeline {
	agent {
              label 'Linux-lab'      
	     }
	stages {
		stage('---clean---') {
			steps {
				tool name: 'Maven3.6.2', type: 'maven'
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				tool name: 'Maven3.6.2', type: 'maven'
                                sh "mvn test"
			}
		}
		stage('---package---') {
			steps {
				tool name: 'Maven3.6.2', type: 'maven'
                                sh "mvn package"
			}
		}
	}
}
         
