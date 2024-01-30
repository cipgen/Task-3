## Git Repository Operations for a Feature Branch

**Clone the Repository with Submodules:**  
Clone the repository using the `--recursive` option to include submodules:  
`git clone --recursive https://github.com/den-vasyliev/gohttps`  
Fetch all branches and updates:  
`git fetch --all`

**Switch to a Specific Feature Branch:**  
Switch to the branch mentioned in the message:  
`git switch -c feature/metrics remotes/origin/feature/metrics`

**Check the Commit Log and Find the Commit Hash with the Fix:**  
Check the commit log:  
`git log`  
(Note: Look for the commit hash, example - d1ac709120)

**Return to the Main Branch:**  
Switch back to the main branch:  
`git checkout main`

**Perform a Cherry-Pick of the Fix Commit:**  
Cherry-pick the commit with the fix:  
`git cherry-pick d1ac709120`

**Review the Modified Code:**  
Check the corrected code in `main.go`:  
`nano main.go`

**Confirm the Changes:**  
Review the log to confirm the changes:  
`git log --oneline`  
(Example output:  
9c4d78f (HEAD -> main) fix default port to 9000  
aa85cde (origin/main, origin/HEAD) improved by GPT  
ae8b3d1 add project description  
94df9be add comments by ChatGPT  
40ee074 init  
