node {
    
  stage 'Checkout'
  git 'https://github.com/vyivrain/docker-wordpress-nginx.git'
  
  stage 'Package Docker image'
  def img = docker.build('vyivrain/docker-wordpress-nginx:latest', '.')

  stage 'Publish'
  println "'${env.BUILD_NUMBER}'"
//   docker.withRegistry('https://registry.hub.docker.com', 'docker-psy') {
//      img.push('latest')
//   }
}
