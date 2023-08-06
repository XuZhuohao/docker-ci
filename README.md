# docker-ci
Use [GitHub Action](https://docs.github.com/zh/actions/quickstart) to build the Dockerfile which from any Repository.

Currently, there are only two actions:
- [Docker image](./.github/workflows/docker-image.yml): from the main branch
- [Docker image pro](./.github/workflows/docker-image-pro.yml): from the tag which is either input or up-to-date.

