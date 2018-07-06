node ('jenkins-maven'){
  try{
    stage 'checkout project'
    container(name:'maven'){
    checkout scm
  
//    stage 'check env'
    sh "mvn -v"
    sh "java -version"

  //  stage 'test'
    sh "mvn test"

    //stage 'package'
    sh "mvn package"


    }
  }catch(e){
    throw e;
  }
}
