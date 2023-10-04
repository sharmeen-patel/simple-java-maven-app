pipeline {   
    agent any
    tools {
        maven 'Maven 3.9.4'
    }
    stages {        
        stage('BUILD'){
          	steps {
      			sh 'mvn clean install site surefire-report:report'
                sh 'tree'
            }
        }
    }
}
