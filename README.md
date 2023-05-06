# ci-cd-pipeline-with-terraform
Project: Complete CI/CD Pipeline with Terraform

1. Create ssh key-pair in aws + add to jenkins credentials

<img width="713" alt="Capture d’écran 2023-05-06 à 10 16 44" src="https://user-images.githubusercontent.com/62488871/236619450-a5da51da-65d5-45b9-84e4-8250d774a68d.png">

<img width="1106" alt="Capture d’écran 2023-05-06 à 10 16 23" src="https://user-images.githubusercontent.com/62488871/236619477-3b15e64b-da6c-403d-8eb6-153a99f2f9a8.png">

2. Install TF inside Jenkins container

<img width="231" alt="Capture d’écran 2023-05-06 à 10 23 38" src="https://user-images.githubusercontent.com/62488871/236619481-68f81aef-30de-4b0b-bdc5-4df63d38d22e.png">

3. Configure TF inside project to provision server

<img width="218" alt="Capture d’écran 2023-05-06 à 12 48 29" src="https://user-images.githubusercontent.com/62488871/236619750-43fafd83-83d0-4769-b2e3-329c22ea2e36.png">

4. Adjust Jenkinsfile

<img width="943" alt="Capture d’écran 2023-05-06 à 12 47 46" src="https://user-images.githubusercontent.com/62488871/236619735-1f9991f6-5db4-4b69-a4fd-f78af2e5fca8.png">

<img width="1009" alt="Capture d’écran 2023-05-06 à 12 48 01" src="https://user-images.githubusercontent.com/62488871/236619738-96dca95d-e25d-4887-873b-eea77aa66fd1.png">

5. Run the pipeline and verify all stages were successful

<img width="1393" alt="Capture d’écran 2023-05-06 à 12 23 08" src="https://user-images.githubusercontent.com/62488871/236619521-b1b5369e-889d-401b-a9e2-d624cdbf7e08.png">

<img width="691" alt="Capture d’écran 2023-05-06 à 12 24 49" src="https://user-images.githubusercontent.com/62488871/236619528-36898fa8-7eb6-46a9-b9fb-e2373bcd074c.png">

<img width="999" alt="Capture d’écran 2023-05-06 à 11 57 24" src="https://user-images.githubusercontent.com/62488871/236619570-e4367496-9dfa-4cb9-b8b0-2dfdcfc17bef.png">

<img width="874" alt="Capture d’écran 2023-05-06 à 11 50 46" src="https://user-images.githubusercontent.com/62488871/236619577-2ff0a390-9927-4798-b989-a46516253359.png">

<img width="813" alt="Capture d’écran 2023-05-06 à 11 57 41" src="https://user-images.githubusercontent.com/62488871/236619594-425f4d66-107f-4d68-963b-cf1e9a96a9ed.png">

<img width="286" alt="Capture d’écran 2023-05-06 à 12 41 36" src="https://user-images.githubusercontent.com/62488871/236619602-2bdf5cd1-fd84-4476-bc60-0310f9fcd056.png">

<img width="487" alt="Capture d’écran 2023-05-06 à 12 28 38" src="https://user-images.githubusercontent.com/62488871/236619618-16aef58e-11a1-49ea-8e66-ce6f45174974.png">

6. Clean up infrastructure

<img width="414" alt="Capture d’écran 2023-05-06 à 12 33 49" src="https://user-images.githubusercontent.com/62488871/236619505-028486c5-ba74-41d0-9b7f-9d86bac88fd3.png">

<img width="653" alt="Capture d’écran 2023-05-06 à 12 34 05" src="https://user-images.githubusercontent.com/62488871/236619507-b42aa4e7-b9fc-4172-9783-9aec4ebc53f4.png">
