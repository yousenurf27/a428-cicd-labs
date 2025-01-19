node {
    stage('Run Build') {
        dockerImage.inside('-p 3000:3000') {
            sh 'npm install'
        }
    }
}