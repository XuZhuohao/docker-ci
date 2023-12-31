# docker-ci
Use [GitHub Action](https://docs.github.com/zh/actions/quickstart) to build the Dockerfile which from any Repository.

Currently, there are only two actions:
- [Docker image](./.github/workflows/docker-image.yml): from the main branch
- [Docker image pro](./.github/workflows/docker-image-pro.yml): from the tag which is either input or up-to-date.
- [java upload release](./.github/workflows/java-upload-release.yml): from the tag which is either input or up-to-date, build java project (maven) and upload jar to the github release page

## How to use
1. Fork this project to your repository.
2. Register a [Docker Hub](https://hub.docker.com/) account.
3. Open your project from step 1.
4. Click the "Settings" tab, and go to "Secrets and variables" -> "Actions".
5. Add Repository secrets, DOCKER_PASSWORD, and DOCKER_USERNAME.
6. Click the "Actions" tab.
7. Input the info and run the action.

if ues [java upload release](./.github/workflows/java-upload-release.yml) you must set the workflow permissions(project -> Settings -> Action -> General -> workflow permissions) like this:
![workflow permissions](./image/workflows_java_upload.png)
