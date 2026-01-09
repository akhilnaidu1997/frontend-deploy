@Library('jenkins-shared-library') _

properties([
    parameters([
        string(name: 'appVersion', defaultValue: ''),
        string(name: 'environment', defaultValue: 'dev')
    ])
])

def configmap = [
    appVersion: (params.appVersion),
    project: "roboshop",
    component: "frontend",
    environment: (params.environment)
]

EKSdeploy(configmap)