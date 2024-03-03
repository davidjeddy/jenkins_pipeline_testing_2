Jenkinsfile (Declarative Pipeline)
pipeline {
    options {
      buildDiscarder(
        logRotator(
          numToKeepStr: '7',
          artifactNumToKeepStr: '7'
        )
      )
    }
    stages {
        stage('stage_1') {
            steps {
              sh '''
                #!/bin/bash -ex
                echo 'starting'
                declare i
                i=0
                while [[ $i -le 10 ]]
                do
                  echo "counter: $i"
                  i=$i+1
                  sleep 10
                done
                echo 'done'
              '''
            }
        }
    }
}
