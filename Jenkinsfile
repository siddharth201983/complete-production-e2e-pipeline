pipeline{
    agent{
        label "jenkins-agent"
    }
    tools{
        jdk 'Java17'
        maven 'Maven3'
    }
    stages("Clean Workspace"){
        steps{
            cleanWs()
        }
    }
    stages("Checkout from SCM"){
        steps{
           git branch: 'main', credentialsId: 'gitcred', url:"https://github.com/siddharth201983/complete-production-e2e-pipeline.git"  
        }
    }
    stages(){
        steps{
            echo "Create Build"
        }
    }
    stages(){
        steps{
            echo "Push Image"
        }
    }
    stages(){
        steps{
            echo "Deployment"
        }
    }
}