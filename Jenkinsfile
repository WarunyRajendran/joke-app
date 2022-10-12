pipeline {
  agent any 

  stages {
    stage('build') {
      steps {
        nodejs{nodeJSInstallationName: '17'} {
          sh "echo 'Building..'"
          sh "pnpm install"
          sh "pnpm run build"
          sh "pnpm test"
      }
    }
  }
}