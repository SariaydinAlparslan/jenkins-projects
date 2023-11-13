# Build and Deploy a Modern YouTube Clone Application in React JS with Material UI 5

![YouTube](youtube-clone-result.png)

https://mrcloudbook.hashnode.dev/youtube-app-deployment-with-gitlab-cicd

### ✨ SG Port ✨

22 80 8080 3000 9000

### ✨ Dockerfile ✨

FROM node:16

WORKDIR /app

COPY package\*.json ./

RUN npm install

COPY . .

RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]

### ✨ GitLab Pipeline ✨

[GitHub](https://github.com/SariaydinAlparslan/pipeline-projects/blob/main/youtube-clone-app/.gitlab-ci.yml)
