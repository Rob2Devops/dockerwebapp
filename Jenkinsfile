node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'DockerHub') {

        def customImage = docker.build("rob2devops/node-web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
