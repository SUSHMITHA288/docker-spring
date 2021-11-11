node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/', 'DockerHub') {

        def customImage = docker.build("docker9686/spring")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
