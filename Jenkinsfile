pipeline{
	agent any 


	stages{
		stage('Compile Stage') {
			steps{
                		withMaven(maven: 'mavenhome') {
				sh 'mvn clean';
			     	}
			}


                   }
                stage('Compile Stage') {
                        steps{
                                withMaven(maven: 'mavenhome') {
                                sh 'mvn compile';
                                }
                        }


                   }


		stage('Testing Stage') {
			steps{
                		withMaven(maven: 'mavenhome') {
				sh 'mvn test';
			     	}
			}


                   }

                stage('Packaging Stage') {
                        steps{
                                withMaven(maven: 'mavenhome') {
                                sh 'mvn package';
                                }
                        }


                   }




	}
}

