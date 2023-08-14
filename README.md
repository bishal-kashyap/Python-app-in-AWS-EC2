# **News Summarizer App deployed in AWS EC2 instance**
![image](https://github.com/bishal-kashyap/Python-app-in-AWS-EC2/assets/142091530/3964a1d4-f479-4fb2-ae83-358e459f60f3)

## Workflow
 - Create an EC2 instance in AWS:
![image](https://github.com/bishal-kashyap/Python-app-in-AWS-EC2/assets/142091530/73fa3862-c2e5-4f4c-933e-1ccae5b960ec)

- Setup inbound rule for port 8501 to allow traffic from the internet:
![image](https://github.com/bishal-kashyap/Python-app-in-AWS-EC2/assets/142091530/f025c3e0-3193-4a00-94fe-0e05996c4981)

- Login into the EC2 instance using the public ip through Git Bash( or using AWS  CLI):
  
  ![image](https://github.com/bishal-kashyap/Python-app-in-AWS-EC2/assets/142091530/8c02fb73-1d39-4619-b0e2-cbe8572508f5)

  ![image](https://github.com/bishal-kashyap/Python-app-in-AWS-EC2/assets/142091530/8fb640ec-80d7-4ba5-9c33-07f8d615ac0e)

- Run below commands to update apt packages and install git:
   ```
   sudo apt update
   sudo apt upgrade
   sudo apt install git
   ```
- Check if git installation is successful or not:
  
   ![image](https://github.com/bishal-kashyap/Python-app-in-AWS-EC2/assets/142091530/271d8d5d-1bad-496e-8266-870eecd109fe)


- Clone this repo containing the app code using:
   ```
  git clone https://github.com/bishal-kashyap/Python-app-in-AWS-EC2.git
   ```
  ![image](https://github.com/bishal-kashyap/Python-app-in-AWS-EC2/assets/142091530/99979932-0981-46bd-a8e6-26c74e929008)

- Install python3 ( if not already installed) and python3-pip :
   ```
    sudo apt install -y python3-pip
   ```
- Install `requirements.txt` to install all other requirements for the python app:
  ```
  python3 -m pip install -r requirements.txt

  ```

- Run the below commands to finally run the application. `nohup` command allows a process to continue running even after we log out of the terminal session :
  
  ```python3 -m streamlit run App.py```
    ![image](https://github.com/bishal-kashyap/Python-app-in-AWS-EC2/assets/142091530/a226d2d1-9034-4362-9504-8367d190745e)

   ```nohup python3 -m streamlit run App.py```
  ![image](https://github.com/bishal-kashyap/Python-app-in-AWS-EC2/assets/142091530/0fa5ee36-ae33-430b-b8d0-a7f82d1d6972)

- To stop the application, take the process id running the python app and kill it:
  
   ``` sudo su | ps -ef ```
  
   ```kill 2378 ```

## **Thanks !**
