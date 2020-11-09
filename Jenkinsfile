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
    }
}
