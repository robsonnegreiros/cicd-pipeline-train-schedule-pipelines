pipeline {
        agent any
        stages {
                state ('Build') {
                        steps {
                                echo 'Running build automation'
                                sh './gradlew build --no-daemon'
                                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
                        }
                }
        }
}
