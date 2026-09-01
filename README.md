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
