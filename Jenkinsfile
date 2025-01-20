pipeline {
    agent any
    stages {
        stage('Setup Node.js') {
            steps {
                // Ensure Node.js is installed
                sh 'node -v'
                echo 'Hello, World!'
            }
        }
        stage('Print Hello World') {
            steps {
                // Create a simple Node.js script to print "Hello, World!"
                writeFile file: 'hello.js', text: '''
                    console.log("Hello, World!");
                '''
                sh 'node hello.js'
            }
        }
    }
}