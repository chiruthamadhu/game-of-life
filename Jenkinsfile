node{
    stage ('scm'){
      git 'https://github.com/chiruthamadhu/game-of-life.git'
      }
      
    stage ('Build & package'){
        sh 'mvn package'
    }
    
    stage ('Results'){
        archive ' gameoflife-web/target/gameoflife.war'
        junit 'gameoflife-web/target/surefire-reports/*.xml'
     }
}
