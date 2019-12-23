pipeline {
	agent {
              label 'Linux-leb'      
	     }
	stages {
		stage('---clean package---') {
			steps {
				tool name: 'Maven3.6.2', type: 'maven'
				sh "mvn clean"
			}
		}
		stage('---test package---') {
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
         
