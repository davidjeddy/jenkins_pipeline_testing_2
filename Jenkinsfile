// https://gist.github.com/merikan/228cdb1893fca91f0663bab7b095757c
pipeline {
    agent any
    stages {
        stage('stage_01') {
            steps {
                sh '''#!/bin/bash
                  echo 'starting'
                  declare i
                  i=0
                  while [[ $i -le 100000000 ]]
                  do
                    echo "counter: $i"
                    i=$(($i + 1))
                    sleep 10
                  done
                  echo 'done'
                '''
            }
        }
    }
}
