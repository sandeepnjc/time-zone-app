pipeline
	{
		agent any
		stages
			{
				stage('Build Application')
					{
						steps
							{
								bat 'mvn clean install -Dmaven.test.skip=true'
							}
					}
				stage('Deploy Application to Cloudhub')
					{
						steps
							{
								bat 'mvn package deploy -DmuleDeploy -Dmaven.test.skip=true'
							}
					}
			}
	}