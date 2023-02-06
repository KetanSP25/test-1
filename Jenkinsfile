pipeline{
		agent{
				label{
						label 'built-in'
						customWorkspace '/mnt/project'
				}
		}
		stages{
			stage('ketan dir'){
					steps{
						sh "rm -rf ketan"
						sh "mkdir ketan"
					}
			
			}
			stage('ketan dir in slave'){
					agent{
							label{
									label 'qa'
									customWorkspace '/mnt/project'
								}
						}
					steps{
						sh "rm -rf ketan"
						sh "mkdir ketan"
					}
			
			}
		
		
		}
		

}
