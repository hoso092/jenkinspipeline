node{
    git branch: 'main' , url:'git@github.com:hoso092/jenkinspipeline.git'
    stage('build'){
        try{
        sh 'echo "Building the project..."'
        }
        catch (Exception e) {
           sh 'echo "Build failed: ${e.message}"'
            throw e
        }
    }
    stage ('test'){
        if (env.BRANCH_NAME == "feat"){
            sh 'echo "test stage"'
        }
        else{
            sh 'echo "test stage not executed"'
        }
    }
}
