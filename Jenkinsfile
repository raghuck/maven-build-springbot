pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
		sh 'mvn package'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Sending email notification....'
                mail body: 'project build successful for job named testpipeline-1',
                from: 'raghu.kumar.ck@gmail.com',
                subject: 'project build successful',
                to: 'raghu.kumar.ck@gmail.com'
            }
        }
    }
}
