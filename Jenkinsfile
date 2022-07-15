pipeline
{
  agent any
  stages {
    stage('Install .Net package') {
      steps {
        sh 'wget https://packages.microsoft.com/config/ubuntu/21.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb'
        sh '''
          sudo dpkg -i packages-microsoft-prod.deb
          rm packages-microsoft-prod.deb
        '''
      }
    }
  }
}
