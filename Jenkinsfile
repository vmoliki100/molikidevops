pipeline {
    agent any
    stages {
	    stage ('Clean Stage') {

            steps {
                withMaven(maven : 'apache-maven-3.6.1') {
                    bat 'mvn clean compile'
                }
            }
        }
		stage ('Build Stage') {
            steps {
                 echo "Hello World!"
                }
        }
    }
}
