pipeline {
    agent any
    stage('Get code from SCM') {
        checkout(
                [$class: 'GitSCM', branches: [[name: '*/master']],
                 doGenerateSubmoduleConfigurations: false,
                 extensions: [],
                 submoduleCfg: [],
                 userRemoteConfigs: [[url: 'https://github.com/kishorepawank/Devlopment']]]
        )
    }

    stage('Composer Install') {
        sh 'echo install'
    }

    stage("PHPLint") {
        sh 'ls -lrth'
    }
}
