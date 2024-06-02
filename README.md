# Git Commit Generator Script

This script is designed to automate the creation of multiple Git commits with specific dates in the past. It can be useful for testing purposes, creating a certain commit history, or for educational demonstrations.

## How It Works

The script performs the following steps:

1. **Imports Required Modules**: 
   - `os` for interacting with the operating system.
   - `random` for generating random numbers.

2. **Loops for 200 Iterations**: 
   - For each iteration, constructs a string representing a number of days ago.
   - Generates a random number between 1 and 11 to represent a random month.

3. **File Modification and Git Commands**:
   - Opens `test.txt` in append mode and writes the string indicating how many days ago the commit represents.
   - Adds `test.txt` to the staging area using `git add`.
   - Commits the changes with a specified date using `git commit`. The date is constructed using the random month and the number of days ago.

4. **Pushes to the Remote Repository**:
   - After all commits are created, pushes the changes to the `main` branch of the remote repository using `git push`.

## Prerequisites

- Git must be installed and properly configured on your machine.
- You must have an existing Git repository initialized.
- Ensure you have write access to the remote repository.

## Usage

1. **Clone your repository**:
   ```bash
   git clone <your-repository-url>
   cd <your-repository-directory>
