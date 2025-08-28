pipeline {
    agent any

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
        stage('Run Java') {
            steps {
                echo "Running the Java application"
                sh 'java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
            }
        }
        stage('Run Python') {
            steps {
                echo "Running the Python script"
                sh 'python3 hello.py'
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
