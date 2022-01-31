pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                sh """
                docker buld -t dock-jen .
                """ 
            }
        }

        stage("run"){
            steps{
                sh"""
                docker run --rm dock-jen
                """
            }
        }
    }
}
