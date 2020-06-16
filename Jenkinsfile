pipeline {
   agent any
   environment {
       BranchName="wishin"
   }
   stages {
      stage('Start build') {
         steps {
            echo 'pwd is now111!'
            //sleep 360
            //sleep 15
            //dir('/var/jenkins_home/workspace') {
               //sh 'ps'
            //}
            echo 'Build runing112312323'
            //sh "pwd"
         }
      }
      stage('Code review'){
         steps {
           echo "This is Codeing......123"
           //sleep 30
           sh "pwd"
           echo "runing master gogogo！！！！"
           sh "ls"
         }
      }
      stage('Test runing'){
         when {
            branch 'wishin'
         }
         steps {
           //sleep 15
           echo "runing testing"
         }
      }
      stage('Deploy ending') {
         environment {Description="This is CHANGE1111!！！！！！"}
         steps{
            script{
               if (env.GIT_BRANCH == 'origin/F2048'){
                  echo "${Description}${BranchName}"
                  //sleep 25
                  sh "ls"
               }
            }
         }
      }
   }
}
