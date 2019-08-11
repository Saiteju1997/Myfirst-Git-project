
node('Node1') {
   def mvnHome
   
      stage('Preparation') { 
      
      git 'https://github.com/Saiteju1997/Maven-Project_demo.git'
          
      mvnHome = tool 'Maven2'
   }
   stage('Build') {
      withEnv(["MVN_HOME=$mvnHome"]) {
         if (isUnix()) {
            sh '"$MVN_HOME/bin/mvn" -Dmaven.test.failure.ignore clean package sonar
         } else {
            bat(/"%MVN_HOME%\bin\mvn" -Dmaven.test.failure.ignore clean package/)
         }
      }
   }
