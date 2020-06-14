pipeline {
   agent any
   stages {
      stage('Analyze with Anchore plugin') {
         steps {
            writeFile file: 'anchore_images', text: 'docker.io/redis:latest'
            anchore name: 'anchore_images'
         }
      }
   }
}