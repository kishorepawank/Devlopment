pipeline {
    agent any
    stages{
        stage('Get code from SCM') {
            steps{
                checkout(
                        [$class: 'GitSCM', branches: [[name: '*/master']],
                         doGenerateSubmoduleConfigurations: false,
                         extensions: [],
                         submoduleCfg: [],
                         userRemoteConfigs: [[url: 'https://github.com/kishorepawank/Devlopment']]]
                )                    
            }

        }

        stage('Composer Install') {
            steps{

                    sh 'echo install'                

            }

        }

        stage("PHPLint") {
            steps{

                    sh 'ls -lrth'                    

            }
            

        }        
    }

}
