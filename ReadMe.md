# GitHub Command Line Tutorial: Clone, Create, Commit, Push to MK4006-A24-DMP Repo (macOS and Windows)

This tutorial provides commands for macOS and Windows to clone the MK4006-A24-DMP repository, create a new document, commit it, and push the changes to the remote GitHub repository.

## Step 1: Clone the Repository

First, clone the MK4006-A24-DMP repository to your local machine.

**For macOS:**

1.  **Open Terminal:**  Open the Terminal application on your Mac (usually found in `/Applications/Utilities`).
2.  **Navigate to the directory:** Use the `cd` command to go to the folder where you want to clone the repository. For example, to use your Documents folder:
    ```bash
    cd Documents
    ```
3.  **Use the `git clone` command:** with the repository URL provided.

    ```bash
    git clone https://github.com/iman-hussain/MK4006-A24-DMP.git
    ```

4.  **Navigate into the cloned repository directory:**
    ```bash
    cd MK4006-A24-DMP
    ```

**For Windows:**

1.  **Open Git Bash:** Open Git Bash from your Start Menu (if you installed Git for Windows).
2.  **Navigate to the directory:** Use the `cd` command to go to your desired folder. For example, to use your Documents folder:
    ```bash
    cd Documents
    ```
    *Note:* In Git Bash, Windows paths might start with `/mnt/c/` for your C drive.

3.  **Use the `git clone` command:** with the repository URL.

    ```bash
    git clone https://github.com/iman-hussain/MK4006-A24-DMP.git
    ```

4.  **Navigate into the cloned repository directory:**
    ```bash
    cd MK4006-A24-DMP
    ```

## Step 2: Create a New Document

Create a new document within your local MK4006-A24-DMP repository folder.

1.  **Use the `touch` command** to create a new file. Replace `<document-name>` with your file name (e.g., `my-assignment.txt`, `report.md`).

    ```bash
    touch <document-name>
    ```

    Example to create a text file named `assignment1.txt`:
    ```bash
    touch assignment1.txt
    ```

    *Note for Windows:* If `touch` is not working in your Windows command prompt, ensure you are using Git Bash. Alternatively, you can create a new file using a text editor and save it directly into your `MK4006-A24-DMP` folder.

## Step 3: Stage and Commit the New Document

Prepare your new document for pushing to the repository.

1.  **Stage the new document:** Use `git add` to add your new file to the staging area. Replace `<document-name>` with your document's name.

    ```bash
    git add <document-name>
    ```

    Example:
    ```bash
    git add assignment1.txt
    ```

    To stage all changes in the current directory, use:
    ```bash
    git add .
    ```

2.  **Commit the staged document:** Use `git commit` with a descriptive message. Replace `"Your commit message"` with a message describing your addition.

    ```bash
    git commit -m "Your commit message"
    ```

    Example:
    ```bash
    git commit -m "Add assignment1.txt document"
    ```

## Step 4: Push to the Repository

Upload your committed changes to the remote GitHub repository.

1.  **Use the `git push` command** to push your local commits to the `main` branch on the `origin` remote.

    ```bash
    git push origin main
    ```

    This will push your changes to the MK4006-A24-DMP repository on GitHub. You might be asked to enter your GitHub username and password or Personal Access Token if it's your first time pushing or if your credentials are not cached.

After completing these steps, your new document will be available in the MK4006-A24-DMP repository on GitHub.

**Summary of Commands (macOS and Windows - use the appropriate terminal as mentioned above):**

```bash
# Step 1: Clone the Repository
cd <your-desired-directory>
git clone https://github.com/iman-hussain/MK4006-A24-DMP.git
cd MK4006-A24-DMP

# Step 2: Create a New Document
touch <document-name>  # Or create using a text editor and save in the repository folder

# Step 3: Stage and Commit the New Document
git add <document-name>  # Or git add . for all changes
git commit -m "Your commit message"

# Step 4: Push to the Repository
git push origin main
