pipeline {
    agent { label "linux" }

    stages {
        stage('Build Docker Container') {
            steps {
                sh """
			        docker build -t ola_mundo .
                """
            }
        }
    	
        stage('Run') {
            steps {
                sh """
                    docker run --rm ola_mundo
                """
            }
        }
    }
}
