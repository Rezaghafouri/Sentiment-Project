# Repository Setup Guide

## Recommended License
For your sentiment analysis project, the **MIT License** is recommended because:
1. It's permissive and business-friendly
2. Allows commercial use
3. Perfect for open-source AI/ML projects
4. Provides liability protection
5. Maintains copyright while allowing others to use your code

Alternative options:
- **Apache 2.0**: If you want additional patent protection
- **GNU GPL v3**: If you want to ensure all modifications remain open source

## Setting Up Your Repository

### 1. Prerequisites
- Install Git from: https://git-scm.com/download/win
- Create a GitHub account: https://github.com

### 2. Creating the Repository on GitHub
1. Go to https://github.com/new
2. Fill in the details:
   - Repository name: `Sentiment-Analysis-Project`
   - Description: "Real-time sentiment analysis system for Iran Khodro using LLM and web search capabilities"
   - Choose "Public" or "Private" (recommended: Public for collaboration)
   - DO NOT initialize with README (we already have one)

### 3. Adding License to Your Project
1. Create a new file named `LICENSE` in your project
2. Copy the MIT License text:
```
MIT License

Copyright (c) [2025] [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### 4. Local Repository Setup
Run these commands in your terminal:
```powershell
# Navigate to your project directory
cd "c:\Users\mrgha\Desktop\Sentiment Project"

# Initialize git repository
git init

# Create and configure .gitignore
echo "__pycache__/" > .gitignore
echo "*.pyc" >> .gitignore
echo ".env" >> .gitignore
echo ".ipynb_checkpoints/" >> .gitignore
echo "sentiment_analysis_results.txt" >> .gitignore

# Add your files
git add .

# Make your first commit
git commit -m "Initial commit: Sentiment Analysis Project with MIT License"

# Add remote repository (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/Sentiment-Analysis-Project.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### 5. Project Structure
Your repository should have this structure:
```
Sentiment-Analysis-Project/
├── LICENSE
├── README.md
├── REPOSITORY_SETUP.md
├── requirements.txt
├── pyproject.toml
└── Sentiment_Analysis/
    └── Sentiment_bot.ipynb
```

### 6. Maintaining Your Repository
- Commit regularly with meaningful messages
- Keep sensitive information (API keys) in `.env` file
- Update requirements.txt when adding new dependencies
- Keep documentation updated

### 7. Best Practices
1. Always pull before starting work
2. Create feature branches for new features
3. Write clear commit messages
4. Review changes before committing
5. Keep the `.env` file in your `.gitignore`

### 8. Collaboration
1. Accept pull requests after code review
2. Use issues for tracking bugs and features
3. Maintain a clean commit history
4. Document significant changes

### 9. Security
- Never commit API keys
- Keep `.env` in `.gitignore`
- Regularly update dependencies
- Review security alerts from GitHub
