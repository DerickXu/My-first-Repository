pipeline {
   agent any
   environment {
       BranchName="wishin"
   }
   stages {
      stage('Start build') {
         steps {
            echo 'pwd'
            //sleep 360
            //sleep 15
            //dir('/var/jenkins_home/workspace') {
               //sh 'ps'
            //}
            echo 'Build runing'
            //sh "pwd"
         }
      }
      stage('Code review'){
         steps {
           echo "This is Codeing......"
           //sleep 30
           sh "pwd"
           echo "runing master"
           sh "ls"
         }
      }
      stage('Test runing'){
         when {
            branch 'wishin'
         }
         steps {
           //sleep 15
           echo "runing test"
         }
      }
      stage('Deploy ending') {
         environment {Description="This is CHANGE!"}
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
