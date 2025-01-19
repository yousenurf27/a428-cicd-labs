node {
    def dockerImage

    stage('Prepare Docker Image') {
        dockerImage = docker.image('node:16-buster-slim')
    }

    stage('Run Build') {
        dockerImage.inside('-p 3000:3000') {
            sh 'npm install'
        }
    }
}