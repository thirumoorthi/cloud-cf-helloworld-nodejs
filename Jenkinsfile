@Library('piper-library-os')
node() {
    stage('prepare') {
        println("Outside class")
        echo "Prepare stage starting"
        checkout scm
        setupCommonPipelineEnvironment script:this
        echo 'Prepare stage Ended.'
    }
    stage('build') {
        echo 'Build stage starting.'
        mtaBuild script: this
        echo 'Prepare stage Ended.'
    }
}
