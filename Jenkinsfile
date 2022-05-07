pipeline { 
    agent any  
    environment{
	PATH="C:/Development/maven-3.6.0/bin"	
    }
    stages { 
        stage('git') { 
            steps { 
                git credentialsId:'git_credentials',url:'https://github.com/rajuraghavan69/recoverydemo.git'
            }
        }
        stage('Build') { 
            steps { 
               echo "mvn clean install"
            }
        }
    }
}
