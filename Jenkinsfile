node{
  
  stage 'Checkout'{
  checkout scm
  }
  
  stage 'Build'{
    
    sh "/.run.sh"
  }
  
  stage 'Deploy'{
    url: 'localhost',
    filename: 'index1.html',
    appid: 'nginx',
    docker: "docker build -t nginx_test:03042018"
  }
}
