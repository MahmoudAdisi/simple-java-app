//Configure the Jenkins Pipeline for this repo with Jenkinsfile type (Declarative)
node{
    git branch: 'main', url: 'https://github.com/DinaGamalMahmoud/simple-java-app.git'
    stage('build'){
        try{
            sh'echo "build stage"'
        }
        catch(Exception e){
            sh'echo "exception found"'
            throw e 
        }

    }
    stage('test'){
        if (en.BRANCH_NAME == "feat"){
            sh'echo "test stage"'
        }
        else{
            sh'echo "skip test stage"'
        }
    }
}
