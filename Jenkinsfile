pipeline {
agent any
stages{
 stage('checkout'){
 steps{
  git 'https://github.com/tisha5al/example/new/master'
  }
 }
 stage('publish){
   steps{
         publishHTML([
         allowmissing:true,
         alwaysLinktoLastBuild:false,
         KeepAll:false,
         reportDir:'.',
         reportFiles:'file.html',
         reportName:'my html page'
      ])

      }
    }
 }
}
