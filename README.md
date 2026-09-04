![logo](https://eliasdh.com/assets/media/images/logo-github.png)
# 💙🤍README🤍💙

## 📘Table of Contents

1. [📘Table of Contents](#📘table-of-contents)
2. [🖖Introduction](#🖖introduction)
3. [📦Extra](#📦extra)
    1. [🖖Info](#🖖info)
    2. [✨Steps](#✨steps)
        1. [👉Step 0: Preparation](#👉step-0-preparation)
        2. [👉Step 1: Clone The GitHub Repository](#👉step-1-clone-the-github-repository)
        3. [👉Step 2: Restore & Build The Project](#👉step-2-restore--build-the-project)
        4. [👉Step 3: Run The Project (Test)](#👉step-3-run-the-project-test)
        5. [👉Step 4: Publish The Project On GCloud](#👉step-4-publish-the-project-on-gcloud)
4. [🔗Links](#🔗links)

---

## 🖖Introduction

I kindly request your thorough examination and absorption of the comprehensive documentation incorporated within the confines of this repository. Your diligent review of the diverse materials provided herein will undoubtedly enhance your understanding of the intricacies and nuances associated with the contents therein.

Please also see following documents:
- [LICENSE](LICENSE.md)
- [SECURITY](SECURITY.md)
- [CONTRIBUTING](CONTRIBUTING.md)

## 📦Extra

### 🖖Info

This is a simple .NET Core web application that displays "Hello, World!" or "Hello AppEngine!". This application is intended to be used as a starting point for creating a .NET Core web application that can be deployed to Google Cloud.

### ✨Steps

#### 👉Step 0: Preparation

- Update and upgrade system
    ```bash	
    sudo apt-get update && sudo apt-get upgrade -y
    ```

- Install the .NET SDK 8.0 or later.
    ```bash	
    sudo apt-get install dotnet-sdk-8.0
    dotnet --version # Check if the installation was successful
    ```
- Insall the Google Cloud CLI [Instructions GCloud CLI](https://github.com/EliasDeHondt/IntegrationProject1-Deployment/blob/main/Documentation/Instructions-GCloud-CLI.md)

- Make sure to create your application first.
    ```bash	
    gcloud app create --region=europe-west1 --project=PROJECT_ID 
    ```

#### 👉Step 1: Clone The GitHub Repository

- Clone the repository
    ```bash
    git clone https://github.com/EliasDeHondt/DotNet-HelloWorld.git
    ```
- Navigate to the project folder
    ```bash
    cd DotNet-HelloWorld
    ```

#### 👉Step 2: Restore & Build The Project

- Restore the project
    ```bash
    dotnet restore
    ```

- Build the project
    ```bash
    dotnet build
    ```

#### 👉Step 3: Run The Project (Test)

- Run the project
    ```bash
    cd HelloWorld.Cloud/
    dotnet run
    ```

- Open a web browser and navigate to `http://localhost:5000` to see the application running.
- Press `Ctrl+C` to stop the application.

#### 👉Step 4: Publish The Project On GCloud

- Publish the project (`This can take a few minutes`)
    ```bash
    gcloud app deploy --quiet
    ```

- You can find your URL at the end of the output of the previous command.
    ```bash
    gcloud app browse
    ```
- Open a web browser and navigate to the URL to see the application running.

## 🔗Links
- 👯 Web hosting company [EliasDH.com](https://eliasdh.com).
- 📫 How to reach us elias.dehondt@outlook.com
