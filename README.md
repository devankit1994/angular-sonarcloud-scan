# Angular Application with SonarCloud Integration

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 17.2.2. It is integrated with SonarCloud for continuous code quality and security analysis. Every push or pull request triggers a GitHub workflow that runs tests, checks code quality, and reports any bugs, code smells, vulnerabilities, and technical debt using SonarCloud.

## Prerequisites

Before running the workflow, ensure you have the following:

- A [SonarCloud](https://sonarcloud.io) account.
- The project key and organization key from your SonarCloud project.
- A **SonarCloud Token** added to your GitHub repository secrets under `SONAR_TOKEN`.

## SonarCloud Setup

1. **SonarCloud Project**: Create a project on [SonarCloud](https://sonarcloud.io/projects/create) linked to this GitHub repository.
2. **SonarCloud Token**: Generate a token from the SonarCloud project and add it as a GitHub secret:

   - Go to your GitHub repository.
   - Navigate to `Settings > Secrets > Actions`.
   - Create a new secret called `SONAR_TOKEN` and paste the token from SonarCloud.

## Workflow Configuration

The repository is set up with a GitHub workflow (`build.yml`) located in `.github/workflows/`. This workflow is triggered on every push or pull request to the `master` branch.

## Project Configuration

The SonarCloud configuration for this project is stored in the `sonar-project.properties` file located at the root of the project:

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
