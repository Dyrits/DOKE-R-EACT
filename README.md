# DOKE-R-EACT

A React app (Create React App) with a Docker setup and a CI/CD workflow deploying to Docker Hub.

## About The Project

A Create React App project with a Docker Compose development setup (web and tests services), a production `Dockerfile`, and a GitHub Actions workflow ("Deploy Frontend") that builds an image, pushes it to Docker Hub and runs the tests inside it on every push to `main`. The app itself is the default Create React App page.

### Built With

- React (Create React App)
- Docker Compose
- GitHub Actions + Docker Hub

## Getting Started

### Prerequisites

- Docker and Docker Compose, or Node.js

### Development

```sh
docker compose up --build    # web on http://localhost:3000, plus a tests service
```

Or without Docker:

```sh
npm install
npm start
npm test
```

## Deployment

The "Deploy Frontend" workflow publishes to Docker Hub on each push to `main`. It currently fails at the Docker Hub login step, which requires a personal access token; the local build and tests pass.

## License

No license file is present in this repository.

## Contact

Dyrits - https://github.com/Dyrits
