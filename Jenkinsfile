pipeline {
  agent any
  stages {
    stage('scan') {
      steps {
        sh "sudo docker run -v ${pwd()}:/src --workdir /src returntocorp/semgrep-agent:v1 semgrep-agent --config p/ci"
      }
    }
  }
}
