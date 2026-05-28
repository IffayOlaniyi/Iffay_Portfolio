# Iffay Portfolio Documentation

## Project purpose
This repository holds a professional personal portfolio site for Iffay Olaniyi. The portfolio is a static HTML/CSS site that presents a concise executive summary of experience, a full resume page, and a polished recruiter-facing design.

## Repository contents
- `index.html` — main portfolio summary page
- `resume.html` — full resume and detailed experience page
- `style.css` — shared styling for the portfolio site
- `profile.jpg` — profile image used on the site
- `.git/` — Git repository metadata

## What was done today
1. Built the portfolio project structure.
2. Created `index.html` with sections for:
   - About
   - Core strengths
   - Selected accomplishments
   - Tools and technologies
   - Contact and resume CTA
3. Created `resume.html` to store the full resume content.
4. Applied clean professional styling in `style.css`.
5. Initialized Git locally and connected to a remote repository.
6. Diagnosed GitHub authentication issues caused by deprecated password authentication.
7. Switched authentication to SSH and configured the correct remote repository.
8. Successfully pushed the portfolio to GitHub.

## GitHub remote repository
The active repository remote is:

- SSH: `git@github.com:IffayOlaniyi/Iffay_Portfolio.git`
- HTTPS: `https://github.com/IffayOlaniyi/Iffay_Portfolio.git`

> Note: the remote repository name uses a capital `P` in `Portfolio`.

## Recommended workflow
Use this workflow on any machine where you edit the portfolio.

### Pull before you edit
```bash
git pull
```

### Edit files
Update `index.html`, `resume.html`, `style.css`, or the profile image.

### Stage changes
```bash
git add .
```

### Commit changes
```bash
git commit -m "Update portfolio content"
```

### Push changes
```bash
git push
```

## Setup steps for a new computer
### 1. Clone the repo with SSH
```bash
git clone git@github.com:IffayOlaniyi/Iffay_Portfolio.git
cd Iffay_Portfolio
```

### 2. If SSH is not set up, use HTTPS with a PAT
```bash
git clone https://github.com/IffayOlaniyi/Iffay_Portfolio.git
cd Iffay_Portfolio
```

Use GitHub username `IffayOlaniyi` and a Personal Access Token (PAT) instead of a password.

## SSH key setup summary
1. Generate a key:
   ```bash
   ssh-keygen -t ed25519 -C "i_olaniyi@outlook.com"
   ```
2. Add the public key to GitHub:
   ```bash
   cat ~/.ssh/id_ed25519.pub
   ```
3. Verify the SSH connection:
   ```bash
   ssh -T git@github.com
   ```
4. Set the remote to SSH if needed:
   ```bash
   git remote set-url origin git@github.com:IffayOlaniyi/Iffay_Portfolio.git
   ```

## How to confirm the remote
```bash
git remote -v
```
Expected output:
```
origin	git@github.com:IffayOlaniyi/Iffay_Portfolio.git (fetch)
origin	git@github.com:IffayOlaniyi/Iffay_Portfolio.git (push)
```

## Troubleshooting
### `Password authentication is not supported`
Use a PAT or SSH. GitHub no longer allows account passwords for Git operations.

### `Repository not found`
- Verify the repo exists on GitHub.
- Verify the owner and repo name are correct.
- Make sure your GitHub account has access to the repo.

### `Host key verification failed`
If you see this when connecting via SSH, type `yes` once and GitHub will be added to your known hosts.

## Future notes
- Keep the portfolio summary in `index.html` and the detailed resume in `resume.html`.
- Use the repository as the single source of truth for updates.
- If you want, publish the repo with GitHub Pages later using the main branch.

## Short reference checklist
1. `git pull`
2. Edit files
3. `git add .`
4. `git commit -m "..."`
5. `git push`
