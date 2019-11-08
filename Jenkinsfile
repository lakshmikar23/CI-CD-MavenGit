node {
	stage('scm checkout')
	{
          git 'https://github.com/lakshmikar23/CI-CD-MavenGit'		  
        }
	stage('compile-package')
	{
		def mvnHome = tool name: 'Maven3.6.2', type: 'maven'
		sh "${mvnHOME}/bin/mvn package"	
	}
}	
	
