
pipeline {
    agent any 
    stages {
        stage('Compile Stage'){
            steps {
                withMaven(maven : 'maven_3_0_5') {
		sh 'mvn test'
		} 
            }
        }
}
}	

        stage('Deployment Stage') { 
            steps {
                withMaven(maven: 'maven_3_0_5){
		steps {
		     withmaven(maven : 'maven_3_0_5'){
	             sh 'mvn test'
		}
            }
        }
        stage('Deploy Stage') { 
            steps {
                withMaven(maven : 'maven_3_0_5'){
		sh 'mvn deploy'
		}
            }
        }
    }
}


