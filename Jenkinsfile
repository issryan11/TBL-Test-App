@Library('Naleem-SharedLibs') _
pipeline{
    agent any
    tools{
       maven "TrustBankBuildTool" 
    }
    stages{
        stage('gitPull'){
            steps{
                sh "echo cloning the code"
                git 'https://github.com/Naleemp/trustBank-prod'
            }
        }
         stage('Build'){
        steps{
            common("Build")
            }
    }
    }
   
}
