pipeline{
  agent any
  
  stages{
  
    stage('Checkout'){    
      steps {
        checkout([$class: 'GitSCM', branches: [[name: '*/Dev']], extensions: [], userRemoteConfigs: [[credentialsId: '74ae08db-ed5b-4d86-8335-ac37ffa208e2', url: 'https://github.com/Jalda-Saikumar/sample-repo.git']]])
      }    
    }
    stage('Building'){    
      steps {
        echo 'Building!'
      }    
    }
    stage('Deploy'){    
      steps {
        echo 'Deploying!'
      }    
    }
  
  }

}
