pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
           echo "build success"
      }
    }
    stage('Test') {
      steps {
          echo "mvn test starts"
      }
    }
    stage('Deploy Development') {
      steps {
            bat "mvn clean package deploy -DmuleVersion=4.4.0 -Dusername=sumedha_March -Dpassword=Lambda=mc2  -DapplicationName=Prc-ins -Denvironment=Sandbox -Dworkers=1 -DworkerType=Micro -Danypoint.platform.client_id=c6b4fa96b2184b3791604b1a6fe211ac  -Danypoint.platform.client_secret=0727E322469341Ffa591e5e5dca1d2bA -DmuleDeploy"
            echo "deploy success"
      }
    }
  }
}