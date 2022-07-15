pipeline {
    agent any

    stage('Install .Net SDK') {
      steps {
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
