node {
    stage('build'){
     echo 'build';
     echo 'master';
    }

    stage('SCM') {
     checkout scm
    }
    stage('SonarQube Analysis') {
     withSonarQubeEnv() {
      sh "./gradlew sonarqube"
     }
    }

    
    stage('test'){
     echo 'testing';
    }
    
    stage('deploy'){
     echo 'deploy';
    }
    
  
}
