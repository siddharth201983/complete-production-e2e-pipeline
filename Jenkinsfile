pipeline{
    agent{
        label "jenkins-agent"
    }
    tools{
        jdk 'Java17'
        maven 'Maven3'
    }
    stages{
        stage("Clean Workspace"){
            steps{
                cleanWs()
            }
        }
        stage("Checkout from SCM"){
            steps{
                git branch: 'main', credentialsId: 'gitcred', url:"https://github.com/siddharth201983/complete-production-e2e-pipeline.git"  
            }
        }
        stage("Build Application"){
            steps{
                 sh 'mvn clean package'
            }
        }
        stage("Test Application"){
            steps{
                 sh 'mvn test'
            }
        }
        stage("Push Image"){
            steps{
                 echo "Push Image"
            }
        }
        stage("Deployment"){
            steps{
                 echo "Deployment"
            }
        }
    }
}
