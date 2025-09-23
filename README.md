# datafun-05-sql

Creating a GitHub account and repository, and setting up a local project to sync with it, is a standard workflow for developers. Here's a step-by-step guide based on your request.

## 1\. GitHub Account and Repository

  * **Create a GitHub Account:** Go to [github.com](https://github.com) and sign up with your email. Follow the on-screen instructions to create your account.
  * **Create a New Repository:** On your GitHub home page, click the **New** button to create a new repository. Name it **`datafun-01-utils`**. You can add an optional description and choose to make it public or private.
  * **Initialize with a README:** It's a good practice to check the "Add a README file" box. This creates an initial file in your repository, which makes cloning easier.

-----

## 2\. Local Setup and Cloning

  * **Create Your Project Folder:** On your computer, open a file explorer and navigate to your `C:` drive. Create a new folder named `Repos`. The full path will be `C:\Repos`.
  * **Clone the Repository:**
      * Open Visual Studio Code.
      * Go to **Terminal** \> **New Terminal** in the top menu.
      * In the terminal, navigate to your new folder by typing `cd C:\Repos`.
      * Now, clone your repository. **Replace** `youraccount` and `yourrepo` with your actual GitHub username and repository name.
        ```
        git clone https://github.com/youraccount/datafun-01-utils.git
        ```
      * After this command, a new folder named **`datafun-01-utils`** will appear inside your `C:\Repos` folder.

-----

## 3\. Adding and Syncing Files

  * **Add `.gitignore` and `requirements.txt`:**
      * In the VS Code file explorer, open the newly created `datafun-01-utils` folder.
      * Create a new file named **`.gitignore`** (make sure there's a dot at the beginning). This file tells Git to ignore certain files and folders, like your virtual environment.
      * Create another new file named **`requirements.txt`**. This file will list all the Python packages your project depends on.
  * **Sync and Save Changes:** In the VS Code terminal, make sure you are in the `datafun-01-utils` folder (`cd C:\Repos\datafun-01-utils`). Then run the following commands in order:
    ```
    git add .
    git commit -m "Add .gitignore and requirements.txt files"
    git push -u origin main
    ```
      * The `git add .` command stages all your changes.
      * The `git commit` command saves a snapshot of your changes with a descriptive message.
      * The `git push` command uploads your changes from your local repository to the remote one on GitHub.

-----

## 4\. Create a Virtual Environment

  * With your terminal still open and your current directory set to `C:\Repos\datafun-01-utils`, run the following command to create a virtual environment:
    ```
    py -m venv .venv
    ```
  * This command creates a new folder named **`.venv`** in your project directory. This folder contains a local, isolated Python environment where you can install packages for this specific project without affecting your system's global Python installation.

-----

