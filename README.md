# React + Vite

Deployment in Amplify based on [AWS tutorial](https://aws.amazon.com/getting-started/hands-on/build-web-app-s3-lambda-api-gateway-dynamodb/) 

In lambdas Check Point Cloud Guard layer will be injected.

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

Domain: 
https://master.dy8rpc2zn4v2u.amplifyapp.com
Repository: aws-serverless-react:master

Pipeline: 
build: npm ci --cache .npm --prefer-offline
deploy: npx ampx pipeline-deploy --branch $AWS_BRANCH --app-id $AWS_APP_ID

after npx ampx sandbox:

Stack ARN:
arn:aws:cloudformation:eu-west-1:642070733164:stack/amplify-awsserverlessreact-root-sandbox-e9809ce8b4/71e94db0-7757-11ef-82e6-06bcb9c52e5f

✨  Total time: 192.94s


[Sandbox] Watching for file changes...
File written: amplify_outputs.json

npx ampx generate graphql-client-code --out amplify/auth/post-confirmation/graphql

Amplify will create the folder amplify/auth/post-confirmation/graphql where you will find the client code to connect to the GraphQL API.

Clean up: In the Amplify console, in the left-hand navigation for the profilesapp, choose App settings, and select General settings. In the General settings section, choose Delete app.
