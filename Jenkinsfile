pipeline {
  agent {
    docker {
      image 'performancetesting/microfocus_onelg_linux_ubuntu:latest'
      args '''-t -i \\
-e "STORM_TENANT=<your tenant id>"  \\
-e "STORM_USERNAME=<your user name>" \\
-e "STORM_PASSWORD=<your password>" \\
--net=host performancetesting/microfocus_onelg_linux_ubuntu'''
    }

  }
  stages {
    stage('StageOne') {
      steps {
        echo 'Hello!'
      }
    }

  }
}