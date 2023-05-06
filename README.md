## Project: Ansible Integration in Jenkins

1. Create dedicated server for Ansible

<img width="1126" alt="Capture d’écran 2023-05-06 à 13 22 16" src="https://user-images.githubusercontent.com/62488871/236636617-a4866d0f-c957-4fbe-9451-3d90856ec62a.png">

2. Install ansible, boto3 and botocore on server, add aws credentials on ansible server too

<img width="474" alt="Capture d’écran 2023-05-06 à 13 23 18" src="https://user-images.githubusercontent.com/62488871/236636642-5dd8da01-f428-453c-bfb1-3a5e1544aae3.png">

<img width="486" alt="Capture d’écran 2023-05-06 à 13 26 36" src="https://user-images.githubusercontent.com/62488871/236636643-255e6f64-4cde-4ac8-87ad-dacb188e1448.png">

3. Create 2 EC2 instances to be managed by ansible

<img width="683" alt="Capture d’écran 2023-05-06 à 13 35 10" src="https://user-images.githubusercontent.com/62488871/236636656-25c068fd-3290-47b7-acf0-c8eedce7aa0c.png">

4. Write ansible files for the project that need to be copied to ansible server - cfg + inventory + playbook

<img width="250" alt="Capture d’écran 2023-05-06 à 14 07 15" src="https://user-images.githubusercontent.com/62488871/236636670-a4f79f74-39dc-41bc-a58d-2ec94193be9f.png">

5. Add stage in Jenkinsfile to copy the files + ssh-key to ansible server

<img width="914" alt="Capture d’écran 2023-05-06 à 14 47 52" src="https://user-images.githubusercontent.com/62488871/236636715-c40cf38f-58fe-4cbd-a0db-472d293aeaca.png">

<img width="1022" alt="Capture d’écran 2023-05-06 à 14 58 16" src="https://user-images.githubusercontent.com/62488871/236636727-4f73b533-74d3-4453-9419-703bcefdd1af.png">

6. Add stage in Jenkinsfile that calls ansible playbook to configure ec2 instances

<img width="967" alt="Capture d’écran 2023-05-06 à 18 47 48" src="https://user-images.githubusercontent.com/62488871/236636774-9591f3c4-ad81-4377-ae70-b152e053dcdb.png">

7. Test that pipeline runs successfully

<img width="446" alt="Capture d’écran 2023-05-06 à 15 09 19" src="https://user-images.githubusercontent.com/62488871/236636796-846d14dd-b3f6-4688-aa75-bcb7ffb4f0d5.png">

<img width="665" alt="Capture d’écran 2023-05-06 à 18 24 23" src="https://user-images.githubusercontent.com/62488871/236636751-a6884a3e-8d25-40cf-be67-5e89e10701b1.png">
