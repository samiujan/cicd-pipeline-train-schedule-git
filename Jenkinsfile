pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                step {
                    echo 'Running Build automation'
                    sh './gradlew build --no-daemon'
                    archiveArtifacts artifacts:dist/trainSchedule.zip
                }
            }
        }
    }
}
