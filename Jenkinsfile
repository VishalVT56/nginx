node{
  
  stage 'Checkout'
  checkout scm
    stage 'Build'
    sh "/.run.sh"
   
   
   
  stage 'Deploy'
    
    url: 'https://localhost'
    appid: 'nginx',
    docker: docker build -t nginx_test
   
}
