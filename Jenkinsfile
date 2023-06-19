pipeline {
    agent any

    stages {
        stage('Build Maven') {
            steps {
		script {
		    M2_HOME='/opt/apache-maven-3.6.3'
		    PATH="$M2_HOME/bin:$PATH"
		    export PATH
		    mvn install
		} 
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
