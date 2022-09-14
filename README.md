# POC Fargate Devtool

## Project node

### Creation steps

Create NX workspace  
`npx create-nx-workspace --name project-node --preset nest --appName my-service --nxCloud false --skipGit true`

### Useful commands

Install dependencies  
`npm i`

Start my-service app  
`nx serve my-service`

Build my-service app in watch mode  
`nx build my-service --watch`