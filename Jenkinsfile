pipeline{

	agent any

	stages
		{
		stage("Build")
			{
				steps 
				{
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
