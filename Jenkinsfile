pipeline {
  agent any
    stages {
        stage('Clean WorkSpace') {
            steps {
                deleteDir ()
                echo 'CleanUp Done'
                  }
				}
		    stage("Checkout") {
            steps {
			    echo 'checkout'
                checkout scm
				          }
              }
			stage("Build") {
            steps {
			    script {
                   sh 'node -v'
                   sh 'npm -v'
                   sh 'npm install'
						}
              }
			}
			stage("Run") {
            steps {
			    script {
                   sh 'npm start'
						}
              }
			}
    }
}
