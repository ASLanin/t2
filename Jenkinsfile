G_giturl = "git@github.com:ASLanin/t2.git"

// just for test 03

properties([
// Builds rotation
    buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '10')),
    disableConcurrentBuilds(),
// Git project
    [$class: 'GithubProjectProperty', displayName: '', projectUrlStr: G_giturl],
// Trigger build from:
    pipelineTriggers([githubPush()])
])

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
