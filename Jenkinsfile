pipeline {
  agent any
  stages {
    stage('scan') {
      steps {
        sh "docker run -v /home/jenkins/workspace/WebGoat:/src --workdir /src returntocorp/semgrep-agent:v1 semgrep-agent --config p/ci"
      }
    }
  }
}
