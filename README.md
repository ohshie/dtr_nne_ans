**Automated Deployment with GitHub Actions & Ansible**

This playbook will allow you to automate the deployment of your application via GitHub Actions. By following this setup, you'll enable seamless CI/CD deployment flows to your remote server using Ansible and Docker.
Prerequisites

Before using the playbook, make sure to configure the following Secrets in your repository settings:
GitHub Secrets

    ACCESS_TOKEN: A fine-grained GitHub Token with access to the necessary repositories.
    REPO_USER: The username of the repository owner.
    SERVICE_REPO: The name of the repository to work with.

Remote Server Secrets

    SERVER_ADDR: The address of the remote server where the application will be deployed.
    SERVER_KEY: The SSH private key for accessing the remote server.
    WORK_FOLDER: The working directory on the remote server (e.g., /home/service/).

Docker Secrets

    DOCKER_NAME: The name for both the Docker image and the running container.
    DOCKER_PORTS: The ports to expose for the Docker container (if required).
    DOCKER_VOLUME: The volumes to mount for the Docker container (if required).
