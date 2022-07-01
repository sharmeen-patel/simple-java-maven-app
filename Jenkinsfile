pipeline
{
	agent any
	
	stages{
		stage('Build')
		{
			steps
			{
				echo "Building App"
			}
		}
		stage('Test')
		{
			steps
			{
				echo "Testing App"
			}
		}
		stage('Deploy')
		{
			steps
			{
				echo "Deploying App"
			}
		}
		
	}
	post
	{
		always
		{
				emailext body: 'Testing jenkins mail functionality with failure scenario', subject: 'Failure from Jenkins', to: 'sharmeeen.patel@outlook.com'
		}
	}
}
