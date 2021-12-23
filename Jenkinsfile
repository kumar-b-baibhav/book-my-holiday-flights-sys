pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
            dir('C:\\Users\\kumarbbaibhav\\projects\\assignment\\book-my-holidays-flights-sys-api') {
                bat 'mvn clean package deploy -DskipMunitTests -DmuleDeploy -DmuleVersion=4.4.0 -Dusername="kumar-baibhav" -Dpassword="Mule@159515" -DapplicationName=book-my-holidays-flights -Denvironment=Sandbox -DbusinessGroup="apisero" -DworkerType=SMALL  -Danypoint.platform.client_id=1ddf475a4f64450896dfb5d84981ea94 -Danypoint.platform.client_secret=84549B409d3D4b91986Ec2BB8962a712'
			}
      }
    }
  }

}