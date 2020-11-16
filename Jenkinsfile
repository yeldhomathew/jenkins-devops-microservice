pipeline {
	agent { docker {image 'maven:3.6.3'}}
	stages  {
	    stage('Build') {
		steps{
		sh 'mvn --version'
		 echo "Build1"}
				}
	stage('Test') {
		steps{
            	 echo "test2"}
		
				}
	stage('integration Test') {
		steps{
             	 echo "test3"}
                
        			}
			}
	post {
		always {
			echo 'im awsome. I run always'
			}
		success {
                        echo 'i run while test success'
                        }
		failure {
                        echo 'i run you fail'
                        }
		changed {
			echo ' changed status'
			}
	}
}
