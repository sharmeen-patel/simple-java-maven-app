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
    post {
        always {
            publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: false, reportDir: 'target/site', reportFiles: 'surefire-report.html', reportName: 'Surefire Report', reportTitles: '', useWrapperFileDirectly: true])
        }
    }
}
