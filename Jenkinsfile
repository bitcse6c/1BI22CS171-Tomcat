pipeline{
	agent any
	tools{
		maven 'Maven'
		jdk 'JDK'
	}
	stages{
		stage('Fetch'){
			steps{
				git "https://github.com/Vinayak-Rajput/1BI22CS190-Tomcat-MavenWebapp.git"
			}
		}
		stage('Build'){
			steps{
				sh "mvn clean package"
			}
		}
		stage('Deploy'){
			steps{
				sh "cp target/MavenWebapp.war /opt/tomcat/webapps"
			}
		
		}
	}
}
