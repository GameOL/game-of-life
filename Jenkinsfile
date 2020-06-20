node {
    stage('scm'){
        git 'https://github.com/wakaleo/game-of-life.git'
    }
    
    stage('build'){
        sh 'mvn package'
    }
  
    stage('Sonar'){
        withSonarQubeEnv('SONAR'){
          sh 'mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.6.0.1398:sonar'
        }
    }
}
