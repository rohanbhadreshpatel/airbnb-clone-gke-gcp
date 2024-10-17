# AirBnb Clone

## Overview

Google Cloud Hosted Enterprise Application for an AirBnb Clone(without booking / date features). The application has a Front Office Portal for customers and a Back Office Portal for customer support.

## Technologies:

- Google Cloud Platform
- MySQL
- Java / Spring
- React.Js
- Docker
- Kubernetes
- Kong API Gateway
- Kubernetes Ingress
- JWT for Authentication

## Architechture Diagram

![Architecture Diagram](images/architecture.png)

## Project Notes

### 1. Functional Requirements

#### Front Office Portal:

- A "Front Office" Web Application that allows customers to:

  - sign-up for accounts,
  - log-in to their account,
  - browse product catalog,
  - place, and pay for orders using credit cards.

#### Back Office Portals:

- A "Back Office" Web Applications that supports customers Queries

- The Back office also has its own backend Spring Boot Application that supports the following functionalities:

  - Viewing & Resolving Customer Queries

### 2. Technical Requirements

The application was implemented in Java Spring and be deployable as Docker Containers on Google Cloud VM's and/or Kubernetes Engine (GKE).

#### Software Stack & Tools

- **Must use Spring Framework (Spring MVC, Spring JPA):**

  - The app uses Spring Framework for **all backend application / services.**
  - For Back Office Portal(s)
  - For REST APIs

  <br/>

- Customer facing Front Office Portal:

  - Utilized **React.js** for Front Office Portal, and used Bootstrap & Material UI for styling components.

  <br/>

- **Development Tools**

  - Builds must be done with Gradle
  - Version of Java should be JDK 11
    <br/>

- **Database & Middleware Requirements**

  - **MySQL Database:** (MySQL database for persisting all data)
    <br/>
  - **RabbitMQ**
    <br/>
  - **Kong API Gateway:** Kong gateway is deployed on GKE ingress, and all services are exposed through the kong gateway.
    <br/>
  - **Credit Card Payments:** Support
    Integration with CyberSource Payment Gateway

### 3. Project images / Demo

#### Front Office Portal

1. Sign Up

   ![Sign Up](./images/sign_up.png)

    <br/>

2. Sign In

   ![Sign In Page](./images/sign_in.png)

  <br/>

#### Back Office Portal

1. Auth Page

   ![Auth Page](./images/backoffice_auth.png)

    <br/>

#### GCP Images

1. Workloads

   ![Workload](./images/gke_workloads.png)

   <br/>

2. GKE Services

   ![GKE Services](./images/gke_service.png)

   <br/>

3. GKE Ingress Details

   ![GKE Ingress Details](./images/gke_ingress.png)

   <br/>

4. GKE MySQL

   ![GKE MySQL](./images/gke_mysql.png)

   <br/>

