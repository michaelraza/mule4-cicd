pipeline {
	agent any
	
	stages {
	
		stage('Build Application') {
			steps {
			
					bat 'mvn clean install'

					}

									}
		stage('Test') {
			steps {

					echo 'Application in Testing Phase…'
					bat 'mvn test'

					}

						}

		stage('Deploy CloudHub') {

					steps {

						echo 'Deploying mule project due to the latest code commit…'
						
						echo 'Deploying to the configured environment….'
						
						bat 'mvn package deploy -DmuleDeploy -Dusername=Michaelraza01 -Dpassword=Welcome007!!! -DworkerType=Micro -Dworkers=1 -Dregion=us-west-2'

							}

						}

					}

				}