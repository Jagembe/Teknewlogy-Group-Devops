# SSH Key Overview

An SSH key is an access credential for the SSH (secure shell) network protocol. This authenticated and encrypted secure network protocol is used for remote communication
between machines on an unsecured open network. SSH is used for remote file transfer, network management, and remote operating system access.

## Pre-requisites:

Created a Github account.

## Implementation Steps:

Logged into Github and created a repository.

Ouput of creating repository in Github.

![image](https://user-images.githubusercontent.com/58337007/150569544-00def2a1-1ab3-4189-9314-ff19c58414e8.png)

Created New SSH Keys as follows:

Navigated to account settings and clicked on the SSH and GPG Keys menu option.

![image](https://user-images.githubusercontent.com/58337007/150570305-c85402cd-802b-43b3-8e27-93016a82c597.png)

Generated ssh key by using the following cmdlet and pressing enter 4 times:

`ssh-keygen`

Output of the above cmdlet.

![image](https://user-images.githubusercontent.com/58337007/150570882-a77a0198-008f-4eb6-8056-94e33b30c244.png)

Displayed the rsa public key by running the following cmdlet:

`sudo cat ~/.ssh/id_rsa.pub`

Output of the above command.

![image](https://user-images.githubusercontent.com/58337007/150571894-7c4ef252-9f52-4b7d-a1b5-647e6d0bf7f0.png)

Copied and added the ssh key to Github as follows:

On Github, clicked on the 'New SSH Key' button.

![image](https://user-images.githubusercontent.com/58337007/150573939-98a66b1f-5d1c-4b4b-9c20-2ffc29d04e5e.png)

![image](https://user-images.githubusercontent.com/58337007/150574532-396e45fc-e195-472b-b6dd-5674db907268.png)

On Github, located the Repo created earlier and copied the ssh Url link:

![image](https://user-images.githubusercontent.com/58337007/150574969-417b9393-f46e-4c67-b2c9-f0a43575682c.png)

On my Terminal, ran the following cmdlet with the url copied from the Github repo to clone the repo:

`git clone git@github.com:Jagembe/Teknewlogy-Group-Devops.git`

Output of the above command.

![image](https://user-images.githubusercontent.com/58337007/150576675-c67e49df-fde4-4b48-870f-a5d5104bd2a5.png)

After Cloning, used teh following cmdlet to show directory-listing.

`ls`

Output of the above command.

![image](https://user-images.githubusercontent.com/58337007/150577136-98b7fce9-b4a5-4673-933b-0b02698843b8.png)

Navigated to the repo folder using the following cmdlet:

`cd Teknewlogy-Group-Devops`

Output of the above cmdlet.

![image](https://user-images.githubusercontent.com/58337007/150577531-9cb42540-cc00-4f5e-846f-6510f942425f.png)

Created a code file with .txt extension using the cmdlet below:

`touch code.txt`

![image](https://user-images.githubusercontent.com/58337007/150577817-8df4e457-c543-4621-8eaa-2dc0110e975b.png)

Opened the .txt file using the follwoing cmdlet:

`nano touch.txt`

Updated it with the follwoing html code:

```
<!DOCTYPE html>
<html>
<body>

<h1>Teknew-Training</h1>

<?php
echo "Hello TeknewlogyGroup DevOps Teams";
?>

</body>
</html>
```

Output of the above commands.

![image](https://user-images.githubusercontent.com/58337007/150578774-8a12238f-5c87-4a91-9ee8-fa66243c876b.png)

Pressed Ctrl+O to save teh code and pressed ENTER, then Ctrl+X to exit the test editor.

Checked if the code was being tracked by git using the following cmdlet:

`git status`

Output of the above command.

![image](https://user-images.githubusercontent.com/58337007/150579412-4eb1d1b5-1d5a-490e-9b35-95adbf693d8f.png)

Used the cmdlet below to have git track the file in the project folder.

`git add .`

Used the cmdlet below to check the status of the staging.

`git status`

Output of the above commands

![image](https://user-images.githubusercontent.com/58337007/150585726-9357edd7-0620-4d1d-af15-730799c20369.png)

Committed the staged changes to the repository using the cmdlet below:

`git commit -m "ssh key demo"

Output of the above comand.

![image](https://user-images.githubusercontent.com/58337007/150586111-7a9b054e-9cee-4962-a613-0ea244a9f216.png)

Pushed the file from the local repository to the remote repository using the cmdlet below:

`git push`

Output of the command above.

![image](https://user-images.githubusercontent.com/58337007/150586612-e57b2b92-f757-423a-a44c-9f33a4cdb28d.png)

Refreshed the Github Repo to display the code file pushed into it.

![image](https://user-images.githubusercontent.com/58337007/150586966-6d32c066-379e-4955-9611-fb522671ef83.png)







