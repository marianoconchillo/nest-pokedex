<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Run in development

1. Clone the repository

2. Run
```
npm install
```

3. Have Nest CLI installed
```
npm i -g @nestjs/cli
```

4. Run database
```
docker-compose up -d
```

5. Clone the ```.env.template``` file and rename the copy as ```.env```

6. Complete the defined environment variables in ```.env```

7. Run the app in dev mode:
```
npm run start:dev
```

8. Rebuild the database using the seed
```
http://localhost:3000/api/v2/seed
```

### Stack
* MongoDB
* Nest

# Production Build
1. Create ```.env.prod```

2. Complete the defined production environment variables

3. Create the new image
```
docker compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```