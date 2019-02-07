pipeline{
  agent any
  stages{
stage("build clean"){
echo "Build clean"
  sh "mvn clean"
}
  stage("Build Package"){
echo "Build packaging"
    sh "mvn package"
}
  stage("Build install"){
    echo "build install"
    sh "mvn install"
  }
  }
}
