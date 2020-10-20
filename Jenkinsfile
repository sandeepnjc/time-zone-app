pipeline
	{
		agent any
		stages
			{
				stage('Unit Test') 
					{ 
      					steps 
      						{
      							bat 'mvn clean test'
      						}
      				}
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