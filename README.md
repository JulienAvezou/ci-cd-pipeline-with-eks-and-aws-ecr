# ci-cd-pipeline-with-eks-and-aws-ecr
Project: Complete CI/CD Pipeline with EKS and AWS ECR

## 1. Create ECR Repository + add ECR repository credentials to Jenkins

<img width="1089" alt="Capture d’écran 2023-05-05 à 23 10 38" src="https://user-images.githubusercontent.com/62488871/236573733-0a9e2f93-ec9c-4842-b69c-27f3e5d8e152.png">

<img width="914" alt="Capture d’écran 2023-05-05 à 23 19 43" src="https://user-images.githubusercontent.com/62488871/236573925-62646ed0-5b9c-4fbd-833a-b9946b6ea676.png">

## 2. Adjust the Jenkinsfile to build and push the Docker image to the ECR repository 

<img width="1238" alt="Capture d’écran 2023-05-05 à 23 14 32" src="https://user-images.githubusercontent.com/62488871/236573755-320139d0-1aa4-4f1b-a798-44c0bc3dca11.png">

- note how it is necessary to specify the repository url in the docker login cmd

## 3. Integrate deploying to k8s cluster in the CI/CD pipeline from AWS ECR repository 

- create k8s secret for ECR + add to the deployment config file

<img width="397" alt="Capture d’écran 2023-05-05 à 23 22 23" src="https://user-images.githubusercontent.com/62488871/236573805-4f727f3e-d70c-4705-b89d-979cf04907ff.png">

<img width="483" alt="Capture d’écran 2023-05-05 à 23 23 41" src="https://user-images.githubusercontent.com/62488871/236573842-106078e0-a63d-4c0a-8591-31d170f0a646.png">

## 4. Verify that the build completes successfully 

- green build

<img width="1356" alt="Capture d’écran 2023-05-05 à 22 57 43" src="https://user-images.githubusercontent.com/62488871/236573965-87376e0b-72b0-41e1-9410-476fa33f7bbe.png">

- the image was built and pushed to ECR repository

<img width="876" alt="Capture d’écran 2023-05-05 à 23 27 11" src="https://user-images.githubusercontent.com/62488871/236573999-77b00c0c-2013-4fe4-b2fc-8cf294d4f7ea.png">

- the image was pulled from ECR repository and deployed in EKS cluster

<img width="376" alt="Capture d’écran 2023-05-05 à 23 29 17" src="https://user-images.githubusercontent.com/62488871/236574043-65a8c113-7135-4f78-aa93-d8e73c3d2786.png">

<img width="461" alt="Capture d’écran 2023-05-05 à 23 37 11" src="https://user-images.githubusercontent.com/62488871/236574097-790e296d-a5ce-4706-800f-e2d7b09bf4e6.png">

- the version update has been committed in github source code repository - note that github now only accepts authentication via personal tokens

<img width="1025" alt="Capture d’écran 2023-05-05 à 23 39 37" src="https://user-images.githubusercontent.com/62488871/236574128-25651bb3-00dd-4c14-ad03-15d7198c6329.png">
