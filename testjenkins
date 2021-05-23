node {
    checkout scm

    docker.withRegistry('https://hub.docker.com', 'DockerHubSecret') {

        def customImage = docker.build("maheshkhade8600/nginx-hello:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
