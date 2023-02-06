pipeline{
		agent{
				label{
						label 'built-in'
						customWorkspace '/mnt/project'
				}
		}
		stages{
			stage('clone master'){
					steps{
						sh "rm -rf *"
						sh "git clone https://github.com/KetanSP25/test-1.git -b master"
					}
			
			}
			stage('clone dev'){
					agent{
							label{
									label 'qa'
									customWorkspace '/mnt/project'
								}
						}
					steps{
						sh "sudo git clone https://github.com/KetanSP25/test-1.git -b dev"
					}
			
			}
		
		
		}
		

}
