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
        stage("Create Build"){
            steps{
                 
            }
        }
        stage("Push Image"){
            steps{
                 
            }
        }
        stage("Deployment"){
            steps{
                 
            }
        }
    }
}