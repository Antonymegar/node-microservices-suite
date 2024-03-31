# Microservices Suite

## Overview

Welcome to the Microservices Suite project! This suite is a collection of node microservices built using the `mono-repo strategy` utilizing the `yarn workspaces` concept. Every `microservice` runs in her `isolated Docker container` and `Kubernetes` is used for `orchestration`, providing fluidity to scaling any service or a combo of services efficiently.

## Features

This suite includes the following microservices:

1. **Enforce DRY principles**: Collocating code encourages code sharing, reduces code duplication as in multi-repo strategy and saves time to scaffold a microservice by building on existing boilerplate or reusable functionality.

2. **Collaboration**: Learning by reading code authored by others as you work within the same repository makes it easier to kick bad habits and pick up some good ones from your peers.

3. **Hoist common development chores**: Manage common files like `.gitignore` from a central place <root-directory> and avoid littering the codebase with unnecessary repetitions. 

4. **Easily integrate developmnent automation**: Manage task runner configurations and docker-compose from <root-directory> to easily automate repetitive workflows.

5. **Code sharing anywhere**: Easily publish and import organization-scoped libraries to the npm registry with `yarn publish` and `yarn add <@microservices-suite/foo>`.

6. **Easily containerize and scale**: Decouple every microservice to scale individually. The `no-hoist yarn workspace` feature of course with our smart scripts to package your `image` enables every microservice to pack all her `astronauts' 🚀 suite to land and explore the moon` 😎.

## Technologies Used
  
- **Yarn Workspaces**: Simplifies managing multiple packages within a single repository, encouraging code sharing, reducing code duplication, and making it easier to handle dependencies and scripts.

- **Docker Containers**: Provides lightweight, portable, and self-sufficient containers for packaging and deploying microservices.
  
- **Kubernetes (k8s)**: Offers automated deployment, scaling, and management of containerized applications, ensuring reliability and scalability.

## Getting Started

To get started with the Microservices Suite, follow these steps:

1. Clone the repository to your local machine:

2. Navigate to the project directory:

3. Install dependencies for all microservices:

4. Follow the individual README files within each microservice directory for specific setup instructions and usage details.

## Contributing

Contributions are welcome! If you'd like to contribute to the Microservices Suite project, please follow these guidelines:

1. Fork the repository and clone it to your local machine.
2. Create a new branch for your feature or bug fix: `git checkout -b feat/<my-feature>` or `git checkout -b fix/<my-bug-fix>`.
3. Make your changes and make sure that tests pass.
4. Commit your changes using the Angular commit message convention:
For more details, please refer to the [Angular commit message convention](https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit).
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
