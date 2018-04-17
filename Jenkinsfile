node {
    def mvnhome
    stage("code checkout") {
        git 'https://github.com/santhosh13nov/course.git'
        mvnhome = tool 'MAVEN_HOME'
    }
    stage("build compile") {
        sh "'${mvnhome}/bin/mvn'  compile"
       
    }
    stage("build test") {
        sh "'${mvnhome}/bin/mvn'  test"
       
    }
    stage("build package") {
        sh "'${mvnhome}/bin/mvn'  package"
       
    }
}
 
