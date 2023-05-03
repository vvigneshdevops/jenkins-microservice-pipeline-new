pipeline{

	// agent { docker { image 'maven:3.6.3'}}
	agent any

	environment {

		mavenHome = tool 'myMaven'
		dockerHome = tool 'myDocker'

		PATH = "$mavenHome/bin:$dockerHome/bin:$PATH"
	}

	stages
		{
		stage("Build")
			{
				steps 
				{
					// sh 'mv --version'
					echo "Build"


					echo "BuildNumber jenkins-${JOB_NAME}-${BUILD_NUMBER}"
					echo "$env.JENKINS_HOME"
					echo "$env.JENKINS_URL"
				}
				
			} 
		stage("Test")
			{
				steps 
				{
					echo "Test"
				}
				
			} 
		
		stage("Integration Test")
			{
				steps 
				{
					echo "Integration Test"
				}
				
			} 
		}

		post
			{
				always{
					echo "I am successfully exec"
				}

				success{
					echo "I am exec success"
				}

				failure{
					echo "I have failed in exec"
				}


			}
}
