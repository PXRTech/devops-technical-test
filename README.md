# devops-technical-test

This is the Pxr Tech GmbH technical assignment for DevOps Engineers.

## The challenge

please setup a production ready and developer friendly Continuous Deployment pipeline for the given demo application.

The demo application can be found in this repository in this [Folder](https://github.com/PXRTech/devops-technical-test/tree/master/devops_tech_test).

the demo code application was created using [Django-cookiecutter](https://github.com/cookiecutter/cookiecutter-django).
refer to this [Documentation](https://cookiecutter-django.readthedocs.io/en/latest/developing-locally.html) for more information.

The requirements are as follows:

- Use (github actions or circleci) as your CI/CD tool.
- Dockerize the whole application to run locally and everywhere in docker containers.
- Setup a continuous deployment pipeline for the containerized demo application.

  - It should contain at least a build, test and a deployment stage.
  - It should only be deployed if the testing stage, which runs the demo applications tests, is successful.

- Setup a 3 environments(dev, staging, production) staging environment which mirrors the production environment as closely as possible.
- Think about scalability and performance.
- User Terraform to setup the infrastructure.(optional - bonus point)
  - setup one ec2 instance that has most of the containers running on it.
  - setup a separate RDS instance for the database
  - make sure the script is idempotent when it comes to environment setup.
- You will need AWS account to finish the task. You can use t2-micro EC2s. Use free tier.

## What to deliver?

- Full Continuous Deployment pipeline.
- Infrastructure setup using Terraform.
- application that we can run using docker-compose up.

you can fork this repository and start working on it.
