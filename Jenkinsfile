pipeline {
    agent any
    stages {
        stage('Prepare') {
            steps {
                // Clean up any previous compilation
                sh 'rm -f SimpleJavaApp.class'
            }
        }
        stage('Compile') {
            steps {
                // Compile the Java file
                echo 'Compiling Java Application...'
                sh 'javac SimpleJavaApp.java'
            }
        }
        stage('Execute') {
            steps {
                // Execute the compiled Java class
                echo 'Executing Java Application...'
                sh 'java SimpleJavaApp'
            }
        }
    }
}
