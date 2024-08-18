# Automated Git uploader

This bash script will upload your project automatically to your Github repository, by simple steps.

## Features

- **Initialize Git Repository** : Automatically initializes a new Git repository if one does not already exist.

- **Set Up Remote URL** : Prompts for the GitHub repository URL and allows updating if a different URL is provided.

- **Commit Message** : prompts everytime when user want to update the repository by pushing the letest code or want to update the code.
- **Push to GitHub** :Adds all changes, commits them with a user-provided message, and pushes them to the `main` branch on GitHub.

- **Update Existing Remote URL** : Updates the remote URL if a new one is provided, or keeps the existing one if no change is desired.

## Requirements

- [Git](https://git-scm.com/) must be installed on your system.
- The script is compatible with Unix-like environments (`Linux`, `macOS`) and can be run using `Git Bash` on Windows.

## Installation

1. Clone the repository.

```
https://github.com/vaghmarelazy/git-automated.git
```

## How to Use

1. In your project directory open the `VScode` terminal by ``` Ctrl+` ```.

2. Clicking on the "+" which trigger a dropdown then select Git bash.


![Select Git bash](https://code.visualstudio.com/assets/docs/sourcecontrol/intro/git-bash.png)

3. Give permission to the script to execute by Git bash
```
chmod +x automation-script.sh
```
4. finally Run the script
```
./automation-script.sh
```
5. After the hitting enter the script ask for the Git repository url and commit message, give that and hit Enter.


### You're Done 🎉

## Script Workflow
1. **Repository Initialization** :
    - Checks if a Git repository is initialized. If not, it initializes one.
2. **Remote URL Management** :
    - Checks if the remote `origin` exists. If it does, it updates the URL if a new one is provided.
    - If the remote `origin` does not exist, it adds the provided URL as the remote repository.
3. **Commit and Push** :
    - Adds all changes, commits them with the provided message, and pushes them to the `main` branch on GitHub.


## Troubleshooting
- __Permissions denied__ : 
    - Ensure the script is executable. Use `chmod +x git-upload.sh` in Unix-like environments.
- __Git Command Not Found__:
    - Make sure Git is installed and available in your system's PATH.
- __URL Already Exists__ :
    - The script updates the existing remote URL if necessary. If you encounter issues, verify the URL configuration using `git remote -v`.

## License

This script is provided as-is without any warranty. Feel free to modify it to suit your needs.