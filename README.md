# Microservices Suite

## Overview

Welcome to the Microservices Suite project! This suite is a collection of microservices built using the monorepo strategy built on top of yarn workspaces concept. It utilizes Docker containers and Kubernetes for orchestration, providing a scalable and efficient solution for various application needs.

## Features

This suite includes the following microservices:

1. **Enforce DRY principles**: Collocating code encourages code sharing, reduce code duplication as in multi-repo strategy and save time to scaffold a microservice by building on existing boiler plate or reusable functionaliy.

2. **Collaboration**: Learning by reading code authored by others as you work within the same repository its easier to kick bad habits and pick up some good ones from your peers.

3. **Hoist common development chores**: Manage common files like `.gitignore` from a central place `<root-directory>`. 

4. **Easily integrate development automation**: Manage task runner configurations and docker-compose from `<root-directory>` to easily automate repetitive workflows.

5. **Code sharing anywhere**: Easily publish and import organization-scoped libraries to npm registry with `yarn publish` and `yarn add @microservices-suite/foo`.

6. **Easily containerize and scale**: Decouple every microservice to scale individually. `no-hoist yarn workspace` feature of course with our smart scripts to package your `image` enables every microservice to pack all her `astronaut 🚀 suite to land and explore the moon` 😎.

## Technologies Used
  
- **Yarn Workspaces**: Simplifies managing multiple packages within a single repository, encouraging code sharing, reducing code duplication, making it easier to handle dependencies and scripts.

- **Docker Containers**: Provides lightweight, portable, and self-sufficient containers for packaging and deploying microservices.
  
- **Kubernetes (k8s)**: Offers automated deployment, scaling, and management of containerized applications, ensuring reliability and scalability.


# Getting Started

Welcome to our project! To ensure a smooth setup and development experience, ensure you have the following tools installed on your machine:

- **Docker:** For containerization and managing containerized applications.
- **Task Runner Automation Tool:** For task automation and workflow management.
- **Node.js:** As the runtime environment for executing the application code.

## Running Services

This project uses a Task Runner Automation Tool to streamline the process of starting services in both development and production. Follow these steps to get your environment up and running:

### Production

To run a service in production:

```bash
task:start:<service_name>
```

This command utilizes docker-compose to orchestrate containers and set up necessary networks using the docker-bridge default network.

### Development
For development purposes, use the following command to start a service, substituting <service_name> with the desired service:

```bash
task:dev:<service_name>
```

The task runner will handle the setup, ensuring your service is ready for development.

### Running Services Without Docker
If you prefer not to use Docker, you can start services using alternative methods:

- - For Production: Start the service with the PM2 engine by running:
#### task vanilla:start:<service_name>
- - For Development: Use the Nodemon node engine for a more development-friendly environment:

#### task vanilla:dev:<service_name>

Using Docker-Compose Directly
Should you need to use docker-compose directly for more control over the container orchestration, you can utilize the standard commands provided by Docker:
```bash
docker-compose up
docker-compose down
```

## Contributing

Contributions are welcome! If you'd like to contribute to the Microservices Suite project, please follow these guidelines:

1. Fork the repository and clone it to your local machine.
2. Create a new branch for your feature or bug fix: `git checkout -b feat/<my-feature>` or `git checkout -b fix/<my-bug-fix>`.
3. Make your changes and ensure that tests pass.
4. Commit your changes using the Angular commit message convention:
Please refer to the [Angular commit message convention](https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit) for more details.
5. Push to the branch: `git push origin feat/<my-feature>` or `git push origin fix/<my-bug-fix>`.
6. Submit a pull request detailing your changes.

Please ensure that your pull request adheres to the project's code style and conventions.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute this code for any purpose.

## Acknowledgements

We would like to thank the developers and contributors to the following technologies used in this project:

- Nx Monorepo Management Framework
- npm Workspaces
- Docker
- Kubernetes
