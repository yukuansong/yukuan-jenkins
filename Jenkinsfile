
node {
    stage('Checkouot code') {
        properties([
            disableConcurrentBuilds(),
            pipelineTriggers([
                cron('H H * * *'),
                pollSCM('H * * * *')
            ])
        ])

        checkout scm
    }
    stage('Build') {
        echo 'Building....'
    }
    stage('Test') {
        echo 'Testing.....'
    }
    stage('Deploy') {
        echo 'Deploying....'
    }
}