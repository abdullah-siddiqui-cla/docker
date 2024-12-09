# Guided Practice: Docker with Express App
## Step 1: Install Docker
## Step 2: Setup a Hello World Express App
Code is already pushed to the repo.
## Step 3: Write a Dockerfile
Create a `Dockerfile` in the same directory as the app.
## Step 4: Build the Docker Image
- Build a Docker image:
```
docker build -t hello-world-app
```
- Verify the image is built:
```
docker images
```
### Step 5: Run the Docker Container
- Run the container from the built image
```
docker run -p 3000:3000 hello-world-app
```
- Open the browser at http://localhost:3000 to see the "Hello, World!" message.

### Step 6: Push Image to Docker Hub
- Log in to Docker Hub via CLI:
```
docker login
```

- Tag the image with their Docker Hub username:
```
docker tag hello-world-app <dockerhub-username>/hello-world-app:latest
```

- Push the image to Docker Hub:
```
docker push <dockerhub-username>/hello-world-app:latest
```

- Verify the image is available on Docker Hub by visiting their repository.


