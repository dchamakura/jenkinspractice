pipeline{
    agent {
         label 'master'
    }
    
    stages{
        
        stage('pull repo'){
            steps {
                git 'https://github.com/gabrielf/maven-samples.git'
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
