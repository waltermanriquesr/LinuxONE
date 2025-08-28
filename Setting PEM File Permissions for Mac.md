# Setting PEM File Permissions
Now, let’s set the permissions on the .pem file we downloaded when we created the SSH key pair

We will start with an example using a mac

In your mac, open a terminal by clicking on Launchpad and then typing Terminal on the search bar

<img width="975" height="268" alt="image" src="https://github.com/user-attachments/assets/32994309-cf71-4d70-938b-4e375bce732a" />

We will assume your browser downloaded content into your ~/Downloads folder

If your browser places the downloaded contented elsewhere, you will have to cd into that folder

The following instructions assume that the browser downloaded the .pem file into $HOME/Downloads folder

In the terminal, issue the cd command to move to the ~/Downloads folder in your home directory, 

cd ~/Downloads

If no errors were reported, you will see the following on the screen

<img width="975" height="196" alt="image" src="https://github.com/user-attachments/assets/2c88fad8-c3e0-4000-bab7-15ad0d0b7544" />

Note that the command completes and no errors are reported

If errors are reported, check that you have no spelling errors

The terminal is case sensitive; did you enter everything using lower case?

Did you capitalize the D in the word Downloads? Did you add or omit a space?

Now, issue the following command replacing the file name part with your own file name to verify the .pem file is in the ~/Downloads directory

ls -l manrique.pem

If no errors are reported, the command will produce output like the following output

<img width="975" height="55" alt="image" src="https://github.com/user-attachments/assets/59dea012-bc1c-4d61-8144-f807e8a3bc11" />

If errors are reported, check that you replaced the .pem file name with your own filename 

Did you use lower case? Did you copy the command correctly? Did you add or omit a space in the command given? Did you use your own .pem file name? 

Once you confirm that the .pem file is present in the ~/Downloads folder, you need to change the permissions on the file using the chmod command

Issue the following command

chmod 600 manrique.pem

If no errors were reported, you are ready to use the .pem file with the ssh command

If you see any errors in the steps above, please repeat them until the steps complete without any errors

You can use the ls -l command again to display your .pem file and verify the new permission for it

<img width="975" height="86" alt="image" src="https://github.com/user-attachments/assets/570549eb-d56d-4c85-b173-7ac72b3fdba5" />

Notice the difference

The previous display had a few extra r characters and now we do not have them

You only need to update the permission on your .pem file once

Now, you are ready to use the .pem file to connect to the virtual machine you created

You will need the machine’s IP address and the .pem file to connect to your virtual machine via ssh
