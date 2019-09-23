node {
    checkout scm 
    /* .. snip .. */
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'kkgowd', url: 'https://github.com/kkgowd/sample_poc.git']]])
}
stage 'build'
node{
    checkout scm
    sh 'mvn clean install'
}


