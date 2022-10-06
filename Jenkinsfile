pipeline {

			agent{
			      label	{
								label 'built-in'
							}

						}
		stages{
			stage('master-1') 
			{
				steps
				{ 
					sh "rm -rf *"
					echo "This is master branch"
					sh "mkdir test"
				}
				
			}
			
			stage('node-1') 
			{
					agent {
			
					label	{
								label '172.31.1.135'
								customWorkspace '/mnt/node-demo'
							}

						}
		
					steps{
					sh "rm -rf *"
					echo "This is Node-1 branch"
					sh "mkdir test"
					}
				
			}
			
			stage('node-2') 
			{
					agent {
			
					label	{
								label '172.31.46.16'
								customWorkspace '/mnt/node2222222222222222222222-demo'
							}

						}
		
					steps{
					sh "rm -rf *"
					echo "This is Node-2 branch"
					sh "mkdir node2-demo"
					}
				
			}
			
		 
			
		}
	}
			
