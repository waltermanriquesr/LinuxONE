# Connecting to LinuxONE form a Mac

To connect to your virtual machine, open a terminal

<img width="975" height="268" alt="image" src="https://github.com/user-attachments/assets/4bcb96d9-d3b5-47d5-9b1d-a133d69b2c8c" />

Now, since the .pem file is in the ~/Downloads directory, we will use the following command to connect to our virtual machine

ssh -i ~/Downloads/manrique.pem linux1@148.100.76.36

<img width="975" height="35" alt="image" src="https://github.com/user-attachments/assets/06c193f8-8c2c-48db-af72-6f9b91ffa0c8" />

The very first time you connect, you will see a prompt, and you will need to answer yes to the prompt

After you reply yes, you will see the following screen

<img width="975" height="624" alt="image" src="https://github.com/user-attachments/assets/87d8a1fb-d648-498a-a2f7-3d7b852ffea5" />

Notice that the exit command was used to terminate the ssh sesison

Now, every time you need to connect to your virtual machine, you only need to open a terminal and enter the ssh command pointing to the correct .pem file

<img width="975" height="619" alt="image" src="https://github.com/user-attachments/assets/5f409dfc-5330-495c-84ab-477d417b081f" />

Remember to always logoff using the exit command all in lower case
