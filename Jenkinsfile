pipeline {   
    agent any
    tools {
        maven 'Maven 3.8.1'
    }
    stages {        
        stage('BUILD'){
          	steps {
      			sh 'mvn clean install site surefire-report:report'
            }
        }
    }
    
}
