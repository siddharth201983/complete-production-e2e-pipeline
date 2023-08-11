pipeline{
    agent{
        label "jenkins-agent"
    }
    tools{
        jdk 'Java17'
        maven 'Maven3'
    }
    stages("Clean Workspace"){
        stage{
            steps{
                cleanWs()
            }
        }
    }
    stages("Checkout from SCM"){
        stage{
            steps{
            git branch: 'main', credentialsId: 'gitcred', url:"https://github.com/siddharth201983/complete-production-e2e-pipeline.git"  
            }
        }
    }
    stages("Create Build"){
        stage{
            steps{
                 
            }
        }
    }
    stages("Push Image"){
        stage{
            steps{
                 
            }
        }
    }
    stages("Deployment"){
        stage{
            steps{
                 
            }
        }
    }
}