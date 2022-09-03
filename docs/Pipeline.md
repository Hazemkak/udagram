# Pipeline

## it contains 3 jobs:

1. Build

- installing node
- Installing frontend dependencies `npm run frontend:install`
- Installing API dependencies `npm run api:install`
- Linting the frontend `npm run frontend:lint`
- Building frontend `npm run frontend:build`
- Building api `npm run api:build`

2. fe-deploy

- Installing node
- Setup aws cli
- Deploying frontend `npm run frontend:deploy`

3. be-deploy

- Installing node
- Setup aws cli
- Setup elastic beanstalk
- Deploying api backend `npm run api:deploy`
