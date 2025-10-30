***For Copying a repo to another repo completely***

```bash
# 1. Go to a folder where you want to store the mirror temporarily
cd ~/Desktop   # or any path you like

# 2. Clone your existing repo (OS) as a mirror
git clone --mirror https://github.com/yourusername/OS.git

# 3. Go inside the mirrored repo directory
cd OS.git

# 4. Add the new remote (CD)
git remote add new-origin https://github.com/yourusername/CD.git

# 5. Push all branches, tags, etc., to the new repo
git push new-origin --mirror
```
