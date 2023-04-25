# Lab Report 1
## Remote Access Instructions

1) Installing VS Code  
I did not have to do this step exactly as I already had VS Code installed on my device, However, the steps that I took to download VS Code were:
- Download the appropiate version of VS Code here: [Link](https://code.visualstudio.com/download)  
![Image](VS_Code_lab1.png)
- Follow steps provided by VS Code to complete download
  
    
2) Remotely Connecting  
During the Lab, my CS 15l account was not working and had to use my regular ucsd account
- Open bash terminal in VS Code  
![Image](Git_Bash_lab1.png)
- Type `ssh cs15lsp23zz@ieng6.ucsd.edu` in the terminal
  - "zz" will be different for every account
  - To find your specific CSE 15L account username, visit: [Link](https://sdacs.ucsd.edu/~icc/index.php)
  - Once Username and Student ID are entered, your `ieng6` account username will be under "Additional Accounts"
  - Press on your account if you wish to change the password, and follow the steps provided
- I had to enter `ssh hriverahernandez@ieng6.ucsd.edu` due to difficulties during the Lab 
- Enter account Password when prompted
- Should see this when complete:  
![Image](VS_Code_Access_Lab1.png)
  
     
3) Trying Commands:
- Here is the list of provided commands:  
  - `cd ~`
    - Changes Working Directory to the Home Directory
  - `cd <directory>`
    - Changes Working Directory to the file provided if the file is inside the Working Dirrectory
  - `ls -lat`
    - Lists all files in Curent Directory, who has permission, and sorts by modification time
  - `ls -a`
    - Lists files in Current Directory
  - `ls /home/linux/ieng6/cs15lsp23/usernmame` where `username` is replaced by another member's CSE 15L account username
    - Lists files in the provided User's Home Direcotry
  - `cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/`
    - Copies files from the provided source
  - `cat /home/linux/ieng6/cs15lsp23/public/hello.txt`
    - Concatinates files from the provided source
  
- Here are the commands I used and their results:  
![Image](Command_Results_lab1.png)

