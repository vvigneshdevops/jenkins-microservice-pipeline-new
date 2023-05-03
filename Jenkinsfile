pipeline{

	agent {docker { image 'maven:3.6.3'}}

	stages
		{
		stage("Build")
			{
				steps 
				{
					sh 'mv --version'
					echo "Build"
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
