pipeline {
  agent any 

  stages {
    stage('build') {
      steps {
          sh "echo 'Building..'"
          sh "pnpm install"
          sh "pnpm run build"
          sh "pnpm test"
      }
    }
  }
}