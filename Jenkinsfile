pipeline
	{
		agent any
		stages
			{
				stage('Build Application')
					{
						steps
							{
								bat 'mvn clean install'
							}
					}
				stage('Deploy Application to Cloudhub')
					{
						steps
							{
								bat 'mvn package deploy -DmuleDeploy'
							}
					}
			}
	}