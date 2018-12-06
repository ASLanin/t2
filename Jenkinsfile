pipeline {
    agent any
        stages {
            stage ('main') {
                steps {
                   script {
                   sh 'ping 8.8.8.8 -c 20'
                   sh 'date'
                }
            }
        }
    }
}
