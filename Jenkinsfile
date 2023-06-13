podTemplate(yaml: '''
    apiVersion: v1
    kind: Pod
    spec:
      containers:
      - name: jnlp
        image: jenkins/jnlp-agent-python
        command:
        - sleep
        args:
        - 99d
''') {
  node('deployment') {
    stage('Get project') {
      git 'https://github.com/adieldevops/test.git'
      container('jnlp') {
        stage('Build') {
          sh 'echo Hi'
        }
      }
    }

  }

}
