pipeline{

    agent any

    stages{

        stage("compile"){

            steps{
            sh 'javac Test.java'
            }
        }

        stage("run"){

            steps{
            sh "java Test"

            }
        }
    }


//this are the post operation in jenkins scripts file
    post{

        always{
            sh 'echo "success'
        }

        success{
            sh 'echo "success"'
        }

        failure{
            sh 'echo "failure"'
        }
    }
}