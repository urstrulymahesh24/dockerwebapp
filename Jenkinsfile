node {

    checkout scm

    docker.withRegistry('https://459155376066.dkr.ecr.us-east-1.amazonaws.com/jenkins', 'dockerHub') {

        def customImage = docker.build("miltonc/dockerwebapp")

        /* Push the container to the d custom Registry */
        customImage.push()
    }
}
