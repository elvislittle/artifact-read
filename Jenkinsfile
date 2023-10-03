pipeline {
    agent any
    stages {
        stage('Read-Artifact') {
            steps {
                copyArtifacts projectName: 'artifact-create',
                    filter: 'report.txt',
                    fingerprintArtifacts: true,
                    selector: lastSuccessful()
            }
        }
    }
}
