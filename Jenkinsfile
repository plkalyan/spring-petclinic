node ('Maven') {

   stage('SCM') {
      // git clone
   git branch: 'main', url: 'https://github.com/plkalyan/spring-petclinic.git'
   }
   
   stage ('build the packages') {
      // mvn package
   sh '/opt/apache-maven-3.8.7/bin/mvn package'
   }
   
   stage ('archival') {
     // archiving artifacts
   archive 'target/*.jar'
   }
}
