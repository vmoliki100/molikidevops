pipeline {
    agent any
    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'apache-maven-3.6.1') {
                    bat 'mvn clean compile'
                }
            }
        }
        stage ('Install Stage') {

            steps {
                withMaven(maven : 'apache-maven-3.6.1') {
                    bat 'mvn install'
                }
            }
        }
        stage ('Deploy Stage') {
            steps {
                withMaven(maven : 'apache-maven-3.6.1') {
                    bat 'deploy'
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
