# React + Vite

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
