@Library('piper-lib-os')
node() {
    
    stages{
        stage('prepare') {
            checkout scm
            setupCommonPipelineEnvironment script:this
        }
        stage('build') {
            mtaBuild script: this
        }
        stage('deploy') {
            cloudFoundryDeploy script: this
       }
    }
}
