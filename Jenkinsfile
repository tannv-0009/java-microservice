node {
   stage('Fetch changes') {
      git 'https://github.com/tannv-0009/java-microservice.git'
   }
   stage('Build images') {
      sh "./package-projects.sh"
   }
   stage('Deploy ECS') {
      sh "./aws-deploy.sh"
   }
}
