pipeline {
    agent any
    stages{
        stage('Get code from SCM') {
            steps{
                step{
                checkout(
                        [$class: 'GitSCM', branches: [[name: '*/master']],
                         doGenerateSubmoduleConfigurations: false,
                         extensions: [],
                         submoduleCfg: [],
                         userRemoteConfigs: [[url: 'https://github.com/kishorepawank/Devlopment']]]
                )                    
                }
            }

        }

        stage('Composer Install') {
            steps{
                step{
                    sh 'echo install'                
                }
                
            }

        }

        stage("PHPLint") {
            steps{
                step{
                    sh 'ls -lrth'                    
                }
            }
            

        }        
    }

}
