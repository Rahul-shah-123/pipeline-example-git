pipeline{

    agent any

    environment{
        VERSION_NAME="1.34"    }


    stages{

        stage("compile"){

            steps{
            sh 'javac Test.java'
            sh 'echo "${VERSION_NAME}"'
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
            sh 'echo "success"'
        }

        success{
            sh 'echo "success"'
        }

        failure{
            sh 'echo "failure"'
        }
    }
}