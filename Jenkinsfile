pipeline {
    agent any

    tools {
        maven 'Maven_3.8.6'   // Replace with your configured Maven tool name in Jenkins
        jdk 'JDK17'           // Replace with your configured JDK in Jenkins
    }

    stages {
        stage('Build') {
            steps {
                echo "Building the project using Maven"
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                echo "Running unit tests"
                sh 'mvn test'
            }
        }
        stage('Run') {
            steps {
                echo "Running the application"
                sh 'java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploy stage (placeholder)"
                sh 'date'
            }
        }
    }
}
