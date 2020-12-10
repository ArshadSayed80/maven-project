pipeline {
    agent any

    //environment{
      //  my_tag = "c:\\temp"
        //my_tag = my_tag
    //}
     
    

    stages{
        stage('Build'){
            steps{
                sh 'sudo mvn clean package'
                sh "sudo docker build . -t tomcatwebapp:${env.BUILD_ID}"
                //bat "echo ${my_tag}"
            }

        }
    }
}
