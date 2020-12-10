pipeline {
    agent any

    //environment{
      //  my_tag = "c:\\temp"
        //my_tag = my_tag
    //}
     
    

    stages{
        stage('Build'){
            steps{
                sh 'mvn clean package'
                sh 'pwd'
                sh 'echo "current working Directory"'
                sh "docker build -f /var/lib/jenkins/workspace/ars-tomcat-web-app/Dockerfile -t tomcatwebapp:${env.BUILD_ID}"
                //bat "echo ${my_tag}"
            }

        }
    }
}
