pipeline {
    agent any

    stages {
        stage('Build Maven') {
            steps {
		   sh "M2_HOME='/opt/apache-maven-3.6.3'"
		   sh 'PATH="$M2_HOME/bin:$PATH"'
		   sh "export PATH"
		   sh "mvn install" 
            }
        }
	stage('Scan With Sonarqube') {
	    steps {
		echo "how are you today"
	   }
	}
	stage('Build Docker') {
	    steps {
		echo "I'm fine, thank you"
	    }
	}
    }
}
