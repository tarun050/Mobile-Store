pipeline{
    agent any stages{
         stage ('checkout the code from SCM'){
             steps{
                 echo 'checkout the code'
                  stage ('Build the project')
                  { steps
                  {echo 'sonar codequality'sh '''
                  mvn clean verify sonar:sonar \ 
                  -Dsonar.projectKey=mobile-store \ 
                  -Dsonar.host.url=http://20.247.104.177:9000 \ 
                  -Dsonar.login=sqp_5d32b6eab1f989a636a4b41a90d5ffa968d06585 '''
                  } 
                  } 
                  }
                  }