node{
  
  stage 'Checkout'{
  checkout scm
  }
  
  stage 'Build'{
    
    sh "/.run.sh"
  }
  
  stage 'Deploy'{
    
    url: 'https://localhost:8080',
    filename: 'index.html',
    appid: 'nginx',
    docker: docker build -t nginx_test
  }
}
