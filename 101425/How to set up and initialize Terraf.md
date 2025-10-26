# How to set up and initialize Terraform



## Quick summary



Install the Terraform binary, add it to your PATH, use a developer terminal (PowerShell / Windows Terminal / Git Bash / WSL), create a small main.tf, run terraform init → terraform fmt → terraform validate → terraform plan → terraform apply. Don’t manually edit .terraform or terraform.tfstate; add state files to .gitignore.





#### Use:



* Windows Terminal or PowerShell (v7+) — for running commands.



* Visual Studio Code — editing .tf files (with the Terraform extension by HashiCorp).



* Git for Windows (gives Git Bash) — for cloning repos and version control.



* (Optional) WSL2 (Ubuntu) if you prefer Linux tooling / scripts.



* Chocolatey (optional) — if you prefer installing Terraform via a package manager.





#### Don’t use:



* Microsoft Word or other rich-text editors to edit .tf files (they add hidden formatting). Use a plain text/code editor (VS Code, Notepad++, or code from VS Code).



* Don’t run Terraform in a random GUI file manager — use a terminal.



* Don’t edit Terraform binary files or vendor provider files directly (see “files not to modify” below).







## Useful Git Bash Commands



| Shortcut      | Description                          |

| ------------- | ------------------------------------ |

| `clear`       | Clear the terminal screen.           |

| `pwd`         | Print current directory path.        |

| `ls`          | List files in the current directory. |

| `cd <folder>` | Change directory.                    |

| `cd ..`       | Move one folder up.                  |

| `git clone    | Clone a repository from GitHub       |









## Step-by-step: initialize a Terraform project



* Open Explorer and create folder you will be working out of.

&nbsp;  ex: mkdir 2025oct14 (In gitbash)



* Open Git Bash (Run as Administrator)



* Find correct path way for working folder

&nbsp;  ex: C:\\Users\\TheoWAF\\class7\\AWS\\Terraform\\2025oct14 (In gitbash)



* Create auth file (In gitbash)

&nbsp;  ex: touch 0-auth.tf 1-main.tf



* Create .gitignore (In gitbash)



* Use command ll



* Open VS Code

&nbsp;   ex: code ./





## Once VS Code opens



* Copy \& Paste 0-auth code from gitbash and place in vs code

&nbsp;   ex: https://github.com/JRobertson7/class7/blob/main/0-Auth.tf



###### \[MAKE SURE FILES ARE SAVED BEFORE OPENING TERMINAL]



* Open up Terminal on VS Code and make sure it is set to Gitbash NOT POWERSHELL using drop down arrow



* &nbsp;^In vs code  curl -O --ssl-no-revoke https://raw.githubusercontent.com/aaron-dm-mcdonald/aws-image-resizer/refs/heads/main/.gitignore



* Initialize the folder - Run terraform init

&nbsp;   \*You should see success message



* Format and validate - Run terraform validate



* See what Terraform plans to do - Run terraform plan



* Apply the plan - Run terraform apply



* To Clean up- Run terraform Destroy











#### Common useful commands



\# check version

terraform -version



\# initialize (download providers)

terraform init



\# reinitialize if needed

terraform init -upgrade



\# validate configuration

terraform validate



\# produce and save a plan

terraform plan



\# apply saved plan

terraform apply 



\# destroy resources

terraform destroy 

