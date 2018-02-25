pipeline{
	agent any 

	stages{
		stage('Compile Stage') {
			steps{
                		withMaven(maven: 'mavenhome') {
				sh 'mvn clean compile';
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


	}
}

