pipeline {
    agent any 
    stages {
        stage('Gradle Build') {
            steps {
                echo 'starting Gradle Build'
                sh './gradlew build --no-daemon'
                archiveArtifacts 'dist/trainSchedule.zip'
            }
        }
    }
}
