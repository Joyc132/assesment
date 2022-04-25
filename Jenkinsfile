pipeline { 
  agent any 
  stages {
    stage ('git clone') {
      steps {
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Joyc132/assesment.git']]])
      }
    }
    stage ('demo') {
      steps {
        sh'''
        test=hi
        echo $test
        '''
      }
    }
  }
}
