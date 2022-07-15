pipeline
{
  agent any
  stages {
    stage('Install .Net package') {
      steps {
        sh 'wget https://packages.microsoft.com/config/ubuntu/21.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb'
        sh '''
              sudo apt-get update; \
              sudo apt-get install -y apt-transport-https && \
              sudo apt-get update && \
              sudo apt-get install -y aspnetcore-runtime-6.0
              sudo apt-get update; \
              sudo apt-get install -y dotnet-sdk-6.0 unzip
              sudo apt-get install zip
        '''
      }
    }
  }
}
