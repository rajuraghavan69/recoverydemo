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
               echo "mvn clean install verify sonar:sonar -Dsonar.login=17c2a8cd16ef28367fb37150d91b12a07c13e1bb"
            }
        }
    }
}
