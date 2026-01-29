pipeline {
    agent {
	node {
	  label "linux && java11"
       }
    }
    stages {
        stage("Hello") {
            steps {
                echo("Hello Pipeline")
            }
        }
    }
    
    post {
	always {
	  echo"I will always say Hello again!"
	}
	success {
	  echo"Yey, success"
	}
	failure {
	  echo"Oh no, failure"
	}
	cleanup {
	  echo"Don't care success or error"
	}
    } 
}
