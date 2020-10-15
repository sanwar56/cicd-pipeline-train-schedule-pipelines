pipeline {
    agent any 
    stages {
        stage('Gradle Build') {
            steps {
                echo 'starting Gradle'
                sh './gradlew build --no-daemon'
                archiveArtifacts 'dist/trainSchedule.zip'
            }
        }
    }
}
