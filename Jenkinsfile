node{
  stage 'Checkout'
  checkout scm
    stage 'Build'
    sh "/.run.sh"
   
    
  stage 'Deploy'
    url: 'https://localhost/',
    filename: 'index.html',
    appid: 'nginx',
    docker: docker run -itd --name Jenkins_vishal_web -p 8080:80 nginx_test
    }
