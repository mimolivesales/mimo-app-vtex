# Mimo API - Apps 
## Sumary
- [Description](#description)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
  - [Install and Config env](#install-and-config-env)
- [Urls](#urls)
- [Commands](#run)
  - [For local env](#for-local-env)
  - [For cloud env](#for-cloud-env)
  - [Generic env](#generic-env)

## Description
A Mimo Live Sales API for satellite apps that allows login, password reset via Cognito and the list of lives of the logged user.

## Prerequisites
- NodeJS for application
  - (the specific version is in the `.tool-version` file)
- Docker for database

## Getting Started
### Install and Config env
 - Run the installation commands in the `terminal`:
 ```
 npm install
 ```
 - Create an `.env` file based on the `.env.example` and ask someone on team for the necessary variable values.

## Urls
 - ___Link___ `/docs` : Open swagger to test API
 - ___POST___ `/auth/login` : To login
 - ___POST___ `/auth/recovery` : Request recovery password
 - ___POST___ `/auth/reset` : Reset password with code
 - ___GET___ `/lives` : List all lives of the logged user
 - ___POST___ `/contact` : Send message to mimo

## Commands
### For local env
 -  To run application
```
npm run start:dev
```
 -  To run tests
```
npm run test:dev
```
 - To generate docs
```
npm run start:doc
```

### For cloud env
 - Run Test in application
```
npm run test
```
 - Run Lint in application
```
npm run lint
```
 - Build application
```
npm run build
```
 - To run application after build
```
npm run start:prod
```

### Generic env
 -  To sync the Prisma with the database
```
npm run db:sync
```