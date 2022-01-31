pipeline{
    agent{ label "linux" }
    stages{
        stage("build"){
            steps{
                sh """
                docker buld -t dock-jen
                """ 
            }
        }

        stage("run"){
            steps{
                sh"""
                docker run --rm dock-jen
            }
        }
    }
}