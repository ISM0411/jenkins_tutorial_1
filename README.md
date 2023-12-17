# jenkins_tutorial_1
Building first Jenkins pipelines

Writing Simple script to test the Jenkins Pipeline working. we are using Docker Agent instead of Configuring mulitple Jenkins Slave node.
we are going to use Pipeline option with pull from SCM options in Jenkins, so that Jenkins will find the Jenkins file from this repository and 
will execute all the steps in the Jenkins file.

### The syntax to write jenkins files:
1. It should start with word pipleline with open and closed curly braces with agent details or none agent
   pipeline{
   agent none
   }
 3. Inside the Piepline should have Stages with open and curly braces
    pipeline{
    agent none
      stages{
     }
    }
 5. And Inside the Stages should have one or multiple stage and followed by one or multi steps on each stage
    pipeline{
    agent none
      stages{
        stage('stage1')
         steps {
         sh ' Hello world'
      }
     }
    }

   few advantage of using Docker Agent in Jenkins are
