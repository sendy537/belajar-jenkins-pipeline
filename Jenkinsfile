pipeline {
    agent {
	node {
	  label "linux && java11"
       }
    }
    stages {
       
	stage("Build") {
            steps {
                echo("Hello Build1")
		sleep(10)
		echo("Hello Build2")
		echo("Hello Build3")
            }
        }
	stage("Test") {
            steps {
                echo("Hello Test1")
		sleep(10)
		pwd(ls)
		echo("Hello Test2")
		echo("Hello Test3")
            }
        }
	stage("Deploy") {
            steps {
                echo("Hello Deploy1")
		sleep(10)
		echo("Hello Deploy2")
		echo("Hello Deploy3")
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

