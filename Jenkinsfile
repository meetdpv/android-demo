  pipeline {
    agent { dockerfile true }
    stages { 
        stage('Build') { 
            steps { 
                // 3
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/meetdpv/android-demo.git']]])
                sh "pwd"
                echo 'SCM Checkout'
            }
        }
       
    }
}  
