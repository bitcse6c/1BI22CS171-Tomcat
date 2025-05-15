pipeline{
	agent any
	tools{
		maven 'Maven'
		jdk 'JDK'
	}
	stages{
		stage('Fetch'){
			steps{
				git "https://github.com/bitcse6c/1BI22CS171-Tomcat.git"
			}
		}
		stage('Build'){
			steps{
				sh "mvn clean package"
			}
		}
		stage('Deploy'){
			steps{
				sh "cp target/mavtom-1.0-SNAPSHOT.war /opt/tomcat/webapps"
			}
		
		}
	}
}
