# POC Fargate Devtool

## Project node

### Creation steps

1. Create NX workspace  
`npx create-nx-workspace --name project-node --preset nest --appName my-service --nxCloud false --skipGit true`

### Useful commands

> Install dependencies  
`npm i`

> Start my-service app  
`nx serve my-service`

> Build my-service app in watch mode  
`nx build my-service --watch`

> Docker build  
`docker build . -t poc-fargate-devtool-project-node`

> Docker run  
`docker run -it -p 5000:3333 --mount type=bind,source="$(pwd)"/dist/apps,target=/home/workspace/apps,readonly poc-fargate-devtool-project-node`
>
> *Now if you build my-service in watch-mode and modify the source-code, app will be automatically restart inside the running container.*