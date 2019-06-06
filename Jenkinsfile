#!/usr/bin/env groovy

try{
  node(){
    if (env.BRANCH_NAME.contains('QA')){
      QATest()
    }
    if (env.BRANCH_NAME.contains('Fusion')){
      FusionTest()
    }
    if (env.BRANCH_NAME.contains('Isolation')){
      IsolationTest()
    }
  }
}
catch(caughtError) {
    throw caughtError
}
finally{

}

def QATest {
  stage("QA test Segment"){
    sh "echo QA"
  }
}

def FusionTest{
  stage("Fusion test Segment"){
    sh "echo Fusion"
  }
}

def IsolationTest {
  stage("Isolation test Segment"){
    sh "echo Isolation"
  }
}
