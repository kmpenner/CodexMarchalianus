# CodexMarchalianus
For StFX Digital Methods for Ancient Manuscripts course
**Title: Introduction to Git for Combining Transcriptions**

**Objective:** In this tutorial, students will learn how to use Git to combine their individual TEI XML transcriptions of Codex Marchalianus. This will provide a collaborative digital environment for working with transcriptions, ensuring effective version control and combining everyone’s contributions into a single, unified file.

---

### **Step 1: Introduction to Git**

Git is a powerful version control system used by many developers and researchers to collaborate on projects. For our purposes, Git will help us track changes to our XML files, manage versions, and merge all individual transcriptions into a consolidated manuscript.

**Why Git?**

- **Version Control:** Git tracks changes, allowing us to revert to earlier versions if needed.
- **Collaboration:** Everyone can work independently on their transcription and easily combine it later.
- **Conflict Resolution:** Git allows us to manage conflicts when multiple people edit the same sections.

### **Step 2: Setting Up Git**

**2.1 Install Git**

- Git can be installed from [Git's official website](https://git-scm.com/).
- Follow the instructions based on your operating system (Windows, Mac, or Linux).

**2.2 Configure Git**

- Open a terminal or command prompt and set up your identity with these commands:
  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "your.email@example.com"
  ```
  Replace "Your Name" and "[your.email@example.com](mailto\:your.email@example.com)" with your actual name and email.

### **Step 3: Clone the Repository**

I have set up a Git repository where we will combine all the XML transcriptions. You will need to **clone** this repository to your computer.

**3.1 Cloning the Repository**

- The shared Git repository for this project is available at [https://github.com/kmpenner/CodexMarchalianus.git.](https://github.com/kmpenner/CodexMarchalianus.git.Use)
- [Use](https://github.com/kmpenner/CodexMarchalianus.git.Use) the following command in your terminal to clone it to your local machine:
  ```bash
  git clone https://github.com/kmpenner/CodexMarchalianus.git
  ```

### **Step 4: Creating Your Branch**

Each student will work in their own branch before combining the transcriptions.

- Navigate into the repository folder:

  ```bash
  cd CodexMarchalianus
  ```

- Create your own branch by using this command:

  ```bash
  git checkout -b your-name-branch
  ```

  Replace `your-name-branch` with something descriptive like your own name, e.g., `ken-transcription`.

### **Step 5: Adding Your Transcription**

**5.1 Copy Your TEI XML File**

- Copy your TEI XML transcription into the cloned repository folder.

**5.2 Add Your File to the Repository**

- In your terminal, add your file to Git:

  ```bash
  git add [YOUR_XML_FILE]
  ```

  Replace `[YOUR_XML_FILE]` with the name of your file.

- Commit your changes with a descriptive message:

  ```bash
  git commit -m "Add transcription of Codex Marchalianus pages 723-726"
  ```

### **Step 6: Push Your Branch**

Next, push your branch to the remote repository so others can see your work.

```bash
git push origin your-name-branch
```

This command will push your branch to the shared repository, making it available for everyone to review.

### **Step 7: Combining Transcriptions (Pull Requests)**

**7.1 Open a Pull Request**

- After pushing your branch, go to the Git repository page (e.g., GitHub) in your browser.
- You should see an option to create a **Pull Request** (PR).
- A Pull Request is a request to merge your changes into the main branch.

**7.2 Review and Merge**

- After everyone has opened a PR, we will review the submissions collectively.
- If there are any conflicts (e.g., two transcriptions editing the same element differently), Git will highlight those, and we will work through resolving them together.

### **Step 8: Pulling the Combined Repository**

Once all transcriptions are merged into the main branch, you can **pull** the latest version of the repository to get the combined transcription.

```bash
git pull origin main
```

### **Step 9: Resolving Merge Conflicts (If Any)**

If you encounter a **merge conflict** when combining transcriptions, Git will indicate which files have conflicts.

- Open the file in your XML editor (Oxygen XML Editor).
- Look for lines marked with `<<<<<<<`, `=======`, and `>>>>>>>` which indicate the conflicting sections.
- Make the necessary corrections to resolve the differences, save the file, and add and commit the resolved file:
  ```bash
  git add [CONFLICTED_FILE]
  git commit -m "Resolve merge conflict in [CONFLICTED_FILE]"
  ```

### **Step 10: Summary and Next Steps**

By following this tutorial, you now understand how to:

- Set up Git on your machine
- Create branches, add your transcription, and push your branch
- Create pull requests to combine all transcriptions

This process is essential for working collaboratively on digital manuscript projects and gives us a consistent and version-controlled way to handle our work.

If you have any issues or questions during this process, please reach out via the discussion board on Canvas or during our next class session.

---

**Next Steps:** Continue working with the merged transcription and start encoding the next phase of annotations as outlined in the upcoming assignment. Make sure to update your local repository frequently using `git pull` to keep up with any changes.

