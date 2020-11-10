@Library('piper-library-os') _
node() {
    stage('prepare') {
        echo "starting stage prepare"
        checkout scm
        setupCommonPipelineEnvironment script:this
        echo "end of stage prepare"
    }
    stage('build') {
        echo "starting stage build"
        mtaBuild script: this
        echo "end of stage build"
    }
}
