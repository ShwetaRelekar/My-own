pipeline {
    agent any 
    stages {
        stage('install') { 
            steps { 
                sh "yum install httpd -y"
            }
        }
        stage('start') { 
            steps {
                sh "service httpd start"
            }
        }
        stage('Deploy') { 
            steps {
                sh "cd /var/wwww/html"
                sh "echo Hello world >> /var/wwww/html/index.html"
                sh "chmod 777 /var/wwww/html/index.html"
              
            }
        }
    }
}
