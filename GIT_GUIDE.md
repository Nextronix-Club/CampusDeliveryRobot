# Git Guide for CampusDeliveryRobot Project

## 📚 Complete Guide for Team Members

### 🔧 Prerequisites
Before starting, make sure you have:
- Git installed on your computer
- GitHub account created
- Access to the repository

---

## 1. 📥 Cloning the Repository

### Option A: Using Command Line (Recommended)
```bash
# Clone the repository
git clone https://github.com/Nextronix-Club/CampusDeliveryRobot.git

# Navigate to the project folder
cd CampusDeliveryRobot

# Check if everything is working
git status
```

### Option B: Using GitHub Desktop
1. Download GitHub Desktop
2. Click "Clone a repository from the Internet"
3. Enter: `Nextronix-Club/CampusDeliveryRobot`
4. Choose your local folder
5. Click "Clone"

---

## 2. 🌿 Creating Your Branch

**Why create a branch?**
- Keeps your work separate from others
- Prevents conflicts
- Allows for easy review

```bash
# Create and switch to your branch
git checkout -b your-name-solution

# Examples:
git checkout -b jeevesh-solution
git checkout -b antra-solution
git checkout -b avani-solution
```

---

## 3. 📝 Making Changes

### Navigate to Your Folder
```bash
cd approach/your-name/
# Example: cd approach/jeevesh-kumar/
```

### Edit Your SOLUTION.md File
1. Open `SOLUTION.md` in any text editor (VS Code, Notepad++, etc.)
2. Write your approach and solution
3. Save the file

### Check Your Changes
```bash
# See what files you've modified
git status

# See the actual changes
git diff
```

---

## 4. 💾 Committing Your Changes

### Stage Your Files
```bash
# Add specific file
git add approach/your-name/SOLUTION.md

# Or add all changes
git add .
```

### Commit Your Changes
```bash
# Commit with a descriptive message
git commit -m "Add my solution approach for CampusDeliveryRobot"

# More specific examples:
git commit -m "Add database design approach by Jeevesh"
git commit -m "Add frontend development strategy by Antra"
git commit -m "Add AI/ML approach for robot vision by Avani"
```

---

## 5. 🚀 Pushing to GitHub

```bash
# Push your branch to GitHub
git push origin your-branch-name

# Examples:
git push origin jeevesh-solution
git push origin antra-solution
```

### First Time Push
If it's your first time, you might need:
```bash
git push -u origin your-branch-name
```

---

## 6. 📮 Creating a Pull Request

### Method 1: GitHub Website
1. Go to: https://github.com/Nextronix-Club/CampusDeliveryRobot
2. You'll see a yellow banner: "Compare & pull request"
3. Click the button
4. Fill in the details:
   - **Title**: "Solution by [Your Name]"
   - **Description**: Brief summary of your approach
5. Click "Create pull request"

### Method 2: Direct Link
After pushing, GitHub will give you a link in the terminal. Click it!

---

## 7. 📋 Pull Request Template

Use this template for your PR description:

```markdown
## Solution by [Your Name]

### My Approach
Brief summary of how I would build the CampusDeliveryRobot

### Key Technologies
- Technology 1
- Technology 2
- Technology 3

### Main Challenges Identified
- Challenge 1
- Challenge 2

### Implementation Steps
1. Step 1
2. Step 2
3. Step 3

### Additional Notes
Any other thoughts or ideas
```

---

## 🆘 Common Issues and Solutions

### Issue 1: "Permission denied"
```bash
# Check if you're in the right directory
pwd

# Make sure you're on your branch
git branch
```

### Issue 2: "Merge conflicts"
```bash
# Get the latest changes
git pull origin main

# Resolve conflicts in your file
# Then commit again
git add .
git commit -m "Resolve merge conflicts"
```

### Issue 3: "Branch already exists"
```bash
# Switch to existing branch
git checkout your-branch-name

# Or create with different name
git checkout -b your-name-solution-v2
```

---

## 🎯 Best Practices

### Commit Messages
- ✅ Good: "Add database schema design approach"
- ❌ Bad: "update file"

### File Organization
- Keep your work only in your assigned folder
- Don't modify other people's files
- Don't change the main README unless asked

### Code Quality
- Write clear explanations
- Use proper markdown formatting
- Include diagrams if helpful

---

## 📞 Need Help?

### Git Commands Reference
```bash
git status          # Check current status
git log             # See commit history
git branch          # List all branches
git pull            # Get latest changes
git push            # Send your changes
```

### Useful Links
- [Git Documentation](https://git-scm.com/docs)
- [GitHub Desktop](https://desktop.github.com/)
- [Markdown Guide](https://www.markdownguide.org/)

---

## 🏁 Quick Workflow Summary

```bash
# 1. Clone (only once)
git clone https://github.com/Nextronix-Club/CampusDeliveryRobot.git
cd CampusDeliveryRobot

# 2. Create branch (only once)
git checkout -b your-name-solution

# 3. Make changes
# Edit your SOLUTION.md file

# 4. Commit and push
git add .
git commit -m "Add my solution approach"
git push origin your-name-solution

# 5. Create Pull Request on GitHub
```

**Good luck with your contributions! 🚀**