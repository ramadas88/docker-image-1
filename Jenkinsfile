node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'ramadas-docker-git-connection') {

        def customImage = docker.build("ramadasm/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
