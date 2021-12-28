pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
         script{
             git credentialsId: '4b22c39f-9efb-4a4f-9662-d23339dc978a', url: 'https://github.com/kumar-b-baibhav/book-my-holiday-flights-sys'
         }
      }
    }
    stage('Build') {
      steps {
            bat 'mvn clean package'
      }
    }
    stage('Deploy') {
      steps {
            bat 'mvn deploy -DskipMunitTests -DmuleDeploy -DmuleVersion=4.4.0 -DgrantType="client_credentials" -DclientId=2e9937aec30b41d3a16c6afa99916280 -DclientSecret=65b08b8bD32540A5a73d5Ae97DFDc792 -DapplicationName=book-my-holidays-flights -Denvironment=Sandbox -DbusinessGroup="apisero" -DworkerType=MICRO '
      }
    }
  }

}
