# **Docker Samples**

This repository contains Dockerfiles for multiple programming languages and frameworks. Each Dockerfile is designed to provide a base image for building and running applications in that language or framework.

## Getting Started

To use one of the Dockerfiles in this repository, simply clone the repository to your local machine and navigate to the directory for the language or framework that you want to use. Then, build the Dockerfile using the `docker build` command. For example, to build the Dockerfile for a Python application, run the following command:

```bash
docker build -t my-app .
```

This will build the Dockerfile and tag the resulting image as `my-app`. You can then use the `docker run` command to run your application in a container.

## List of Dockerfiles

- [JavaScript](javascript/)
  - [Node](javascript/node/)
    - [Dockerfile](javascript/node/Dockerfile)
  - [React](javascript/react)
    - [Dockerfile.dev](javascript/react/Dockerfile.dev)
    - [Dockerfile.prod](javascript/react/Dockerfile.prod)
- [Elixir](elixir/)
  - [Dockerfile](elixir/Dockerfile)
- [Python](python/)`
  - [Django](python/django)
    - [Dockerfile](python/django/Dockerfile)

## Contributing

We welcome contributions to this repository! If you would like to contribute a Dockerfile for a new language or framework, or if you have found a bug in an existing Dockerfile, please follow the guidelines in the [CONTRIBUTING.md](CONTRIBUTING.md) file.

## License

This project is licensed under the MIT License. Please see the [LICENSE](LICENSE) file for more information.

## Contact

If you have any questions or comments about this project, please feel free to [open an issue](https://github.com/AashishChakravarty/docker-samples/issues/new) in the repository or contact the project maintainers directly.
