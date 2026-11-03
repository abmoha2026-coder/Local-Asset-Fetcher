# Local-Asset-Fetcher
is a lightweight Bash utility that automates the downloading of public repositories and configuration files, automatically organizing them into categorized folders based on their file extension.

Features
Auto-Categorization: Automatically sorts downloads into specific folders:
repos_git/ 
→
→ Git repositories
scripts_py/ 
→
→ Python files
configs_yml/ 
→
→ YAML/YML files
data_json/ 
→
→ JSON files
Smart Detection: Differentiates between a git clone operation and a curl file download.
Clean Workspace: Prevents root directory clutter by creating organized sub-directories.

Installation
1. Prerequisites
Ensure you have curl and git installed on your Linux system:

sudo apt update && sudo apt install curl git -y
setup
chmod +x fetch.sh

Usage
Pass the URL of the file or repository you wish to fetch.Example: Cloning a Repository
bash


./fetch.sh 


: Saved to ./repos_git

. /fetch.py https://github.com/user/repo.py

Result Saved to /repos_py

fetch.sh htpps://github.com/user/repo.yml

Saved yp /repo_py


