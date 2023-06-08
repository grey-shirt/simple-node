def imageName = 'grey-shirt/simple-node'

node('workers'){
    stage('Checkout'){
        checkout scm
        }

    stage('Build Image'){
        def imageTest= docker.build("${imageName}",
        "-f Dockerfile .")
    }
}
