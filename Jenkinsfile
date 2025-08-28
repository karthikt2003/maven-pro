pipeline {
    agent any

    tools {
        maven 'mvn-local'   // Use your actual configured Maven tool name
        jdk 'jdk-local'     // Use your actual configured JDK name
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
                sh 'java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
            }
        }
    }
}
