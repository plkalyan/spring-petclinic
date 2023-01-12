node ('Maven') {

   stage('SCM') {
      // git clone
   git branch: 'main', url: 'https://github.com/plkalyan/spring-petclinic.git'
   }
   
   stage ('build the packages') {
      // mvn package
   sh 'mvn package'
   }
   
   stage ('archival') {
     // archiving artifacts
   archiveArtifacts artifacts: 'target/*.jar', followSymlinks: false
   }
}
