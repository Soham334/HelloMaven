node {

    stage('Checkout') {
        echo 'Checking out source code...'
        checkout scm
    }

    stage('Build') {
        echo 'Starting Build...'
        bat 'mvn clean package -DskipTests'
    }

    stage('Test') {
        echo 'Starting Tests...'
        bat 'mvn test'
    }

    stage('Deploy') {
        echo 'Starting Deployment...'
        bat 'echo Deployment completed successfully - Webhook Test'
    }
}