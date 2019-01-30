pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        awsCodeBuild envVariables: '[ { RUN_TESTS, false } ]', projectName: 'build_trusty_python2_library', region: 'us-east-1', sourceControlType: 'jenkins', credentialsType: 'keys'
      }
    }
  }
}
