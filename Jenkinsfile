pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building something..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing something..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying something..'
            }
        }
		
		 stage('test data pipeline') {
                when {changeset "data_pipeline/*.*" }

                steps {
                    echo 'Testing data pipeline..'
                }
            }
    }
}
