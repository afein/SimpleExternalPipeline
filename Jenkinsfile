#!groovy

properties([pipelineTriggers([pollSCM('')])])

node() {
   
   stage('CHECKOUT') { 
      checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'c1d172c2-6118-4233-8cf3-90029ebcf007', url: 'https://github.com/afein/subversion-plugin']]])
   } 
    
   stage('BUILD') {
      echo 'in build stage'
   }

   stage('REPORTS') {
      echo 'REPORTS'
   }
}
