

![Netflix-clone OverView img](https://github.com/Jagan-18/Netflix-clone/assets/97144563/0f7759c3-7f82-46d4-a760-492888a26fd4)


## Steps:-
- We will be using Jenkins as a CICD tool and deploying our application on a Docker container and Kubernetes Cluster and we will monitor the Jenkins and Kubernetes metrics using Grafana, Prometheus and Node exporter

# Step 1 — Launch an Ubuntu(22.04) T2 Large Instance

# Step 2 — Install Jenkins, Docker and Trivy. Create a Sonarqube Container using Docker.

# Step 3 — Create a TMDB API Key.

# Step 4 — Install Prometheus and Grafana On the new Server.

# Step 5 — Install the Prometheus Plugin and Integrate it with the Prometheus server.

# Step 6 — Email Integration With Jenkins and Plugin setup.

# Step 7 — Install Plugins like JDK, Sonarqube Scanner, Nodejs, and OWASP Dependency Check.

# Step 8 — Create a Pipeline Project in Jenkins using a Declarative Pipeline

# Step 9 — Install OWASP Dependency Check Plugins

# Step 10 — Docker Image Build and Push

# Step 11 — Deploy the image using Docker

# Step 12 — Kubernetes master and slave setup on Ubuntu (20.04)

# Step 13 — Access the Netflix app on the Browser.

# Step 14 — Terminate the AWS EC2 Instances.


<div align="center">
  <a href="http://netflix-clone-with-tmdb-using-react-mui.vercel.app/">
    <img src="./public/assets/netflix-logo.png" alt="Logo" width="100" height="32">
  </a>

  <h3 align="center">Netflix Clone</h3>

  
</div>



<br />

<div align="center">
  <img src="./public/assets/home-page.png" alt="Logo" width="100%" height="100%">
  <p align="center">Home Page</p>
  <img src="./public/assets/mini-portal.png" alt="Logo" width="100%" height="100%">
  <p align="center">Mini Portal</p>
  <img src="./public/assets/detail-modal.png" alt="Logo" width="100%" height="100%">
  <p align="center">Detail Modal</p>
  <img src="./public/assets/grid-genre.png" alt="Logo" width="100%" height="100%">
  <p align="center">Grid Genre Page</p>
  <img src="./public/assets/watch.png" alt="Logo" width="100%" height="100%">
  <p align="center">Watch Page with customer contol bar</p>
</div>

## Prerequests

- Create an account if you don't have on [TMDB](https://www.themoviedb.org/).
  Because I use its free API to consume movie/tv data.
- And then follow the [documentation](https://developers.themoviedb.org/3/getting-started/introduction) to create API Key
- Finally, if you use v3 of TMDB API, create a file named `.env`, and copy and paste the content of `.env.example`.
  And then paste the API Key you just created.




## Install with Docker

```sh
docker build --build-arg TMDB_V3_API_KEY=your_api_key_here -t netflix-clone .

docker run --name netflix-clone-website --rm -d -p 80:80 netflix-clone
```

## Todo

- Make the animation of video card portal more similar to Netflix.
- Improve performance. I am using `context` and `provider` but all components subscribed to the context's value are re-rendered. These re-renders happen even if the part of the value is not used in render of the component. there are [several ways](https://blog.axlight.com/posts/4-options-to-prevent-extra-rerenders-with-react-context/) to prevent the re-renders from these behaviours. In addition to them, there may be several performance issues.
- Replace bundler([Vite](https://vitejs.dev/guide)) with [Turbopack](https://turbo.build/pack/docs/why-turbopack). Turbopack is introduced in Next.js conf recently. It's very fast but it's nor ready to use right now. it just support Next.js, and they plan to support all others as soon as possible. so if it's ready to use, replace [Vite](https://vitejs.dev/guide) with [Turbopack](https://turbo.build/pack/docs/why-turbopack).
- Add accessibilities for better UX.
- Add Tests.




## For Refel Url's : 
   - https://mrcloudbook.com/netflix-clone-ci-cd-with-monitoring-email-devsecops/#more-1831
   - https://www.youtube.com/watch?v=pbGA-B_SCVk
     
