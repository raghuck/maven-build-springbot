pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
			rtMaven.run pom: 'pom.xml', goals: 'package'
			    }
            }
        }
    }
}
