## Project Overview

This project deploys a full-stack Movie Application to an Amazon EKS cluster using Kubernetes and automated CI/CD pipelines with GitHub Actions.

The application consists of:

- A React frontend
- A backend API
- Kubernetes Deployments and Services
- Amazon EKS
- Amazon ECR
- AWS Elastic Load Balancers
- GitHub Actions CI/CD workflows

The frontend communicates with the backend through the backend Kubernetes LoadBalancer service.

---

## CI/CD Pipeline Screenshots

### Frontend Pipelines

#### Frontend CI
![Frontend CI](https://drive.google.com/file/d/10KbdKAKVMtuXs8Fq8OMC2gQGqoLHirsp/view?usp=sharing)

#### Frontend CD
![Frontend CD](https://drive.google.com/file/d/1eKFWvd2RiNofsVB3WHbOEduZWRPZe1pf/view?usp=sharing)

### Backend Pipelines

#### Backend CI
![Backend CI](https://drive.google.com/file/d/18-wMxd3peOzLwLj40vyL5mib7eeB0QvY/view?usp=sharing)

#### Backend CD
![Backend CD](https://drive.google.com/file/d/1erB7HcdkYR0Z2YgimruXX76aNbwvIxpu/view?usp=sharing)

---

## GitHub Repository

Public GitHub Repository:

https://github.com/soumojit622/upgraded-train

---

## Application URLs

### Frontend

http://a0bef39a25c034cdf93b742e4c9a7545-1341005237.us-east-1.elb.amazonaws.com

The frontend provides the Movie List and Movie Details interface.

### Backend

http://aeb24bbf5b57a4179b1ea6d1f0f89cef-481818325.us-east-1.elb.amazonaws.com

Backend API endpoint:

http://aeb24bbf5b57a4179b1ea6d1f0f89cef-481818325.us-east-1.elb.amazonaws.com/movies

The `/movies` endpoint returns the available movies.

---

## Example Movie Data

The backend currently returns:

```json
{
  "movies": [
    {
      "id": "123",
      "title": "Top Gun: Maverick"
    },
    {
      "id": "456",
      "title": "Sonic the Hedgehog"
    },
    {
      "id": "789",
      "title": "A Quiet Place"
    }
  ]
}
