pipeline{
    agent {
         label 'master'
    }
    
    stages{
        
        stage('pull repo'){
            steps {
               
            }
        }
        stage('build'){
            steps {
                sh 'mvn clean package'
            }
        }
        stage ('print') {
           steps {
              sh 'echo $BUILD_ID'
           }
        }
    }
        
}
