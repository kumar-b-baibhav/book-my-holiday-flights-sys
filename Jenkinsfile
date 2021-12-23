pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
            dir('C:\\Users\\kumarbbaibhav\\projects\\assignment\\book-my-holidays-flights-sys-api') {
                bat 'mvn clean package deploy -DskipMunitTests -DmuleDeploy -DmuleVersion=4.4.0 -DgrantType="client_credentials" -DclientId=2e9937aec30b41d3a16c6afa99916280 -DclientSecret=65b08b8bD32540A5a73d5Ae97DFDc792 -DapplicationName=book-my-holidays-flights -Denvironment=Sandbox -DbusinessGroup="apisero" -DworkerType=MICRO '
			}
      }
    }
  }

}