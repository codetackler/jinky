pipeline {
  agent any
  triggers {
    upstream(upstreamProjects: "janky/master",
             threshold: hudson.model.Result.SUCCESS)
  }
  stages {
    stage('Junky') {
      steps {
        sh '''
            echo "Hasta La Vista"
            sleep 90
        '''
      }
    }
  }
}
