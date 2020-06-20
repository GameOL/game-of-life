node {
  stage ('source'){
    git 'https://github.com/GameOL/game-of-life'
  }
  
  stage ('build'){
    sh 'mvn package'
  }
  
}
