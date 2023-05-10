pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        // Checkout source code from your github
        // Build application such as (e.g ., Maven, Gradle etc)
        sh 'mvn clean install'
      }
    }
    stage('Test') {
      steps {
        // Run your tests
        sh 'mvn test'
      }
    }
    stage('Deploy') {
      steps {
        // Deploy your application (e.g., to a web server, container, etc.)
        sh 'mvn deploy'
      }
    }
  }
}
