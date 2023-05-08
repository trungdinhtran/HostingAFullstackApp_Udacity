## Pipeline

![Pipeline](pipeline.png)

### Continuous Integration
#### GitHub
In a big project build with Github, a lot of branch is crated. We are using the CircleCI to trigger one of all branch to build and deploy automatic. The CircleCI is linked with the Github and auto build and deploy the newest code version to AWS S3 and AWS ElasticBeanstalk commit automatic when code is pushed to the repository.

- **Frontend Task**: Runs the `frontend:build` script given in the `package.json` file to build.
- **API Task**: Runs the `api:build` script given in the `package.json` file to build.
- **On hold**: Waiting to accept the build is success and confirm to deploy.
- **Deploy hold**: Runs the `deploy` script given in the `package.json` file to deploy both API and front-end.