pipeline{
    agent any
    
    environment{
        PATH = "/opt/maven3/bin:$PATH"
    }
    
    stages{
        stage("Git Checkout") {
            steps{
                git 'https://github.com/patilnishant789/my-app'
            }
        }
        stage("Maven Build") {
            steps{
                sh "mvn test"
            }
        }
    }
}
