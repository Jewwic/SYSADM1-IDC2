

|  SCHOOL OF INFORMATION AND TECHNOLOGY |  |  |
| ----- | :---- | :---: |
| NAME: Jerric Panayo | DATE PERFORMED: November 21, 2024 |   |
| Section: IDC2 | DATE SUBMITTED: November 21, 2024 |  |

1. # SYSADM1 – Git Basics

Answer the following research questions about Git, GitLab desktop and GitHub.

1. What is Git, and why is it important in software development?

Git is an open-source version control system used to manage source code. It allows developers to track changes in their projects, collaborate on code, and maintain a history of all updates. This ensures efficient teamwork and safeguards against accidental data loss by enabling restoration of previous versions of a project.

2. How does Git track changes in a project?

Git tracks changes by creating snapshots of files during commits. Each snapshot records the current state of the project along with metadata like commit messages, author details, and timestamps. This structure forms a chain of commits, offering a complete history of the project.

3. What is the difference between a local repository and a remote repository in Git?

* **Local Repository:** Stored on an individual developer's computer, allowing private, offline work.

* **Remote Repository:** Hosted on a server (e.g., GitHub or GitLab) and accessible to team members for collaboration and version synchronization.

4. What are the basic Git commands?

* git add – Stage files for commit

* git branch – Manage branches

* git clone – Clone a remote repository

* git commit – Save changes

* git init – Initialize a repository

* git log – View commit history

* git merge – Combine branches

* git pull – Download updates from a remote repository

* git push – Upload changes to a remote repository

* git status – Display repository state

5. How do you check the status of a Git repository?

Use the command git status. It shows staged, unstaged, and untracked files, providing a clear overview of the repository's current state.

6. What is the purpose of branches in Git, and how do you create and switch between them?

Branches allow developers to work on different features or fixes independently. 

To create and switch we can do the following:

* Create a Branch: git branch \<branch-name\>

* Switch to a Branch: git checkout \<branch-name\>

Alternatively:

* Create and Switch Simultaneously: git checkout \-b \<branch-name\>

7. What are GitLab Desktop and GitHub, and how are they different from Git?

GitLab and GitHub are platforms for hosting Git repositories, providing tools for collaboration, versioning, and DevOps. GitHub, Focuses on community collaboration and open-source projects. While GitLab, Offers integrated CI/CD pipelines and enterprise-level DevOps solutions.

8. How do you connect a local Git repository to a GitLab or GitHub repository?

Here are the steps to connect a local Git repository to a remote repository on GitLab or GitHub:

* First, we Initialize the local repository: git init

* Second, we add the remote URL: git remote add origin \<repository-URL\>

* And Lastly, we push changes: git push \-u origin master

9. What are the steps to collaborate with others using GitLab or GitHub?

To start collaborating on a project, first clone the repository using git clone \<repository-URL\>. Once you have the repository on your local machine, create a new branch for your work with git checkout \-b \<branch-name\>. Make the necessary changes to the files, then stage and commit them using git add \<file-name\> followed by git commit \-m "message" to save your changes. After committing, push your branch to the remote repository with git push origin \<branch-name\>. Finally, open a pull or merge request to propose your changes for code review and approval.

10. How do you resolve merge conflicts in Git?

To resolve merge conflicts in Git, start by running git status to identify the files that have conflicts. Next, open the conflicted files and manually edit them to resolve the discrepancies. Once you've resolved the conflicts, stage the changes with git add \<file-name\>. After staging the files, commit the resolved changes using git commit. Finally, push the updates to the remote repository with git push origin \<branch-name\>.

11. What is a pull request, and why is it used in GitHub?

A pull request proposes merging changes from one branch into another. It facilitates collaboration by enabling code reviews, discussions, and approval workflows before integration.

12. What are some best practices for writing commit messages?

* Be concise and clear.

* Keep the subject line under 50 characters.

* Provide context or reasoning in the body if needed.

* Reference relevant issues or tickets.

* Use the imperative mood (e.g., "Add feature" instead of "Added feature").