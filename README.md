# AWS DevOps CICD Pipeline

![AWS Archi drawio](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/36441eb4-7221-4c7b-8754-0f24d4ac48aa)

## Create CodeCommit Repo
![1](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/73bc5622-844b-4df9-b6b6-66a5f7b8ad52)

![3](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/b3a4f2f2-23c4-41fe-9b82-a359f41a0bc1)

![2](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/c57d77b6-9a5b-4379-9214-7a4ecb3fa19c)

## Create CodeBuild

![cb-1](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/a553ae82-f524-4a61-b252-6de2466f9f2b)

![cb-2](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/195a11ab-302a-4175-ad47-1c587b6c2000)

![cb-3](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/c24357e9-aace-41c2-b92c-d54535b53947)


![5 5](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/8d86d35d-6abf-41da-ae30-7a47bc09a133)

![5](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/9d4c0210-bfa4-44aa-bd44-44f0083efec8)

![4](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/e0268707-a864-471e-92cb-9c6fad0683a5)

![4 4](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/1ca675f7-8fa3-4390-bd05-307945d431ad)

### DockerHub Repo
![3 3](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/6f947019-6c52-41f8-98d7-677b260cc08a)

![6](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/14ad0dc8-5e6c-4174-8607-4753f134c47e)

## Create CodeDeploy Application

![cd-1](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/82f15955-9633-441e-91ef-5550303a8b09)

### Create Ec2 instance

![ec2-1](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/d10584f0-c0c0-4222-bc33-de27e5d06b99)

![ec2-2](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/113fe3f3-26cf-47f8-a58e-e63ef7447a6d)

![ec2-3](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/4d99e6ab-555c-4251-a515-174c50954c35)

```bash
#!/bin/bash
sudo yum -y update
sudo yum install -y docker
sudo service docker start
sudo usermod -aG docker ec2-user
sudo yum -y install ruby
sudo yum -y install wget
cd /home/ec2-user
wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
sudo chmod +x ./install
sudo ./install auto
```
- For Ubuntu
  
```bash
#!/bin/bash
sudo apt update
sudo install docker.io
sudo apt install ruby-full
wget cd /home/ubuntu wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
chmod +x ./install
sudo ./install auto
sudo service codedeploy-agent status
```

![27](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/57099108-8944-4335-8af7-dcdd21c7697f)

### Create CodeDeploy Group

![cd-2](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/e15a042b-6e9d-49d5-a759-5ddc99bc6e2d)

![cd-3](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/9911ef67-e5c0-47e3-a6dc-cd505ded21f6)

![10](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/467279df-33fe-4f4d-a25c-434881928f9b)

## Create CodePipeline

![30](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/496d8613-dd1d-4805-8cb3-cb1964e31747)

![31](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/ee10d299-f46b-4112-b27c-056e8fc1c516)

![8](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/8676878e-6b10-4f6a-97cd-a320b760488e)

![11](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/77c56809-aaa7-4668-9914-186f3312c69d)

![12](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/46fb5cd4-8e46-48e5-be22-4155160cc131)

![32](https://github.com/darjidhruv26/AWS-CICD-Pipeline/assets/90086813/469a3d2f-7bb0-4f70-beaf-da4427e0a0e4)

s3://netflix-cicd-arti/netflix.zip
```
