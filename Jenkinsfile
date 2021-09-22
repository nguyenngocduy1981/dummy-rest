pipeline {
	agent { docker { image 'maven:3.3.3' } }
	stages {
		stage("build") {
			steps {
				sh 'mvn --version'
				sh 'mvn clean install'
			}
		}
		stage("test") {
			steps {
				echo 'Dang test app nhe'
			}
		}
		stage("deploy") {
			steps {
			    sh 'mvn package'
				echo 'Dang deploy app nhe'
			}
		}
	}
}
