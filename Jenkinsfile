node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhublogin') {

        def customImage = docker.build("makelinuxinteresting/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
