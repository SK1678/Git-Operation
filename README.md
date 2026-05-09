# Git Operations

## Git Desktop Basics
### Download Git
- Download Git from the official website and install it on your computer. <a href="https://git-scm.com/downloads" target="_blank">Git Download</a>

## Installation Steps (Windows)
1. Open the download link
2. Click **Download for Windows**
3. Run the installer
4. Keep default settings
5. Click **Install**
6. Finish installation
   
### Verify Installation
Open **Command Prompt** or **Git Bash** and run:

```bash
git --version
```
Example output:

```bash
git version 2.49.0.windows.1
```

### Configure Git
```bash
git config --global user.name "User Name"
git config --global user.email "your@email.com"
```
### Check configuration:
```bash
git config --list
```
## GitHub Basics

### Create Repository On GitHub:
- New Repository
- Repository name
- Repo Type: Public or Private
- Create

### Connect Local Project to GitHub
- Go to local project root folder and open cmd or access trough cmd directly
```bash
cd project folder name
```
- Initialize Git to peoject folder:
```bash
git init
```
- Output: It will create a **.git/** folder to the local project root.
- Connect Repository
 ```bash
 git remote add origin https://github.com/username/repo.git
```
- You can check Status by:
```bash
git status
```
- You can add a single file by
```bash
git add file name
```
- Or  all of root 
```bash
git add .
```
- Commit changes:
```bash
git commit -m "Commit Notes"
```
- Push Change:
```bash
git push -u origin branchName
```
### Create and Switch Branches
- Create Branch:
```bash
git branch branchName
```
Output: It will create the branch according to branch name 
- Switch Branch:
```bash
git switch -c branchName
```
Output: It will will shwitch the default push/ pull branch
- Push Change:
```bash
git push -u origin branchName
```
# Git Pull Push workflow
<table>
  <tr>
    <th>Initial Push</th>
    <th>Initial Pull</th>
  </tr>
  <tr>
    <td>Flow the process if repo is not connected:
      <ul> 
        <li>git init</li>
        <li>git add .</li>
        <li>git commit -m "Initial commit"</li>
        <li>git remote add origin git@github.com:username/portfolio.git</li>
        <li>git push -u origin BranchName</li>
      </ul>
    </td>
     <td>Flow the process if repo is not connected 
     <ul>
       <li>**Direct HTTP Pull:** git clone https://github.com/username/project.git</li>
     </ul>
     </td>
  </tr>
  <tr>
    <th>Initial Push</th>
    <th>Initial Pull</th>
  </tr>
</table>
