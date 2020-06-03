pipeline{

    environment {
        registry = "grigciulache/httpd"
        registryCredential = 'dockerhub'
        projectGit='https://github.com/grigciulache/hellosh.git'
    } 
    agent any
    stages{
        stage("Git clone"){
            steps{
                echo 'Git clone'
                git projectGit
            }
        }
        
        stage('Run Application'){
            steps{
                    sh label: '', script: 'echo "hello from sh"'
            }
        }
    }
}
