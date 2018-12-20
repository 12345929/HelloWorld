node{
    
    stage("check out code from Git"){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/smoothwood/HelloWorld.git']]])
    }
    stage("execute"){
        dir('C:\\YCM\\TEMP\\jenkins\\JenkinsHome\\workspace\\MyFirstPipeline') {
            bat("python HelloWorld.py")
        }
    }
    stage("deploy"){
        echo "deploy stage"
    }
    stage("release")
    {
        echo "release stage!!!"
    }
    stage("test"){
        echo "test stage!!!"
    }
    stage("whatever"){
        echo "whatever"
    }
}