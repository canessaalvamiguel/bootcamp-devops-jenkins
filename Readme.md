# Jenkins
This repository demonstrates how to set up a Jenkins service in a Docker container and connect it with the Docker host.

## Prerequisites

- Docker installed (https://docs.docker.com/desktop/install/windows-install/)
- Docker Compose installed (https://docs.docker.com/compose/install/)

# Steps
1. Clone this repository.

2. Navigate to the jenkins directory:
```bash
cd jenkins
docker-compose up --build
```

3. Open your web browser and navigate to http://localhost:8080 (Jenkins default port).

4. Follow the on-screen instructions to complete the Jenkins setup.

5. Create a new pipeline in Jenkins.

6. Connect the pipeline to this repo: https://github.com/canessaalvamiguel/bootcamp-devops-jenkins

7. Click the "Build Now" button to trigger the pipeline build.

## Note:

This is a basic example. You may need to configure Jenkins further based on your specific needs.
Additional Resources

Docker documentation: https://docs.docker.com/
Docker Compose documentation: https://docs.docker.com/compose/
Jenkins documentation: https://www.jenkins.io/doc/