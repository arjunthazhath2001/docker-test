# Manual Installation
- Install nodejs locally
- Clone the repo 
- Run npm install - to install dependencies
- Start the DB locally:
    - docker run -e POSTGRES_PASSOWRD=mysecret -d -p 5431:5432 postgres
    - get one from neon db
- Change .env file and update DB credentials
- npx prisma migrate dev
- npx prisma generate
- npm run dev


# Docker Installation
- Install docker
- Start postgres
    - docker run -e POSTGRES_PASSWORD -d -p 5431:5432 postgres
- Build the image:
    - `docker build -t myapp .`
- Start the container:
    - `docker run -d -p 3000:3000 myapp`


# Docker Compose Installation