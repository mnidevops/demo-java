pipeline
{
	agent any
	stages
	{
		stage('CheckOut')
		{
			steps
			{
				git credentialsId: 'GIT_CREDENTIALS', url: 'https://github.com/mnidevops/demo-java.git'
			}
		}
		stage ('Print branch name')
		{
			steps
			{
				sh 'echo $BRANCH_NAME'
			}
		}
		stage ('Unit testing stage')
		{
			steps
			{
				echo "This is a unit testing stage"
			}
		}	
	}
}
