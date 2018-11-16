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
    }
}
