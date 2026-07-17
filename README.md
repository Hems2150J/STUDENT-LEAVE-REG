# Student Leave Management System

A web-based Student Leave Management Portal designed for HODs and department administrators to manage and log student leaves.

## Features
- **Interactive Dashboard**: Search student profiles instantly by Roll Number, Register Number, or Name.
- **Detailed Profiles**: Browse student general info, family details, academic records, and bank information.
- **Leave Entry & Logs**: Log new leaves and view/filter the history of student leaves.
- **Excel Integration**: Import student data dynamically from local spreadsheets (`.xlsx` / `.xls`) and export leave logs to Excel.

---

## Local Database Privacy
The student database Excel sheet (`CYBER.xlsx`) is listed in `.gitignore` to prevent confidential student records from being pushed to public git repositories. 

---

## How to Host on Vercel

This is a single-page static application. You can host it on Vercel for free in a few simple steps:

### Option 1: Deploy via GitHub (Recommended)
1. **Create a GitHub Repository**: Create a new repository on GitHub (private is recommended for leave administration apps).
2. **Commit and Push Your Code**:
   ```bash
   git add .
   git commit -m "Prepare for Vercel deployment"
   # Link your local repository to your GitHub repository and push:
   git remote add origin <your-github-repo-url>
   git branch -M main
   git push -u origin main
   ```
3. **Import to Vercel**:
   - Log in to your [Vercel Dashboard](https://vercel.com).
   - Click **Add New** > **Project**.
   - Import your GitHub repository.
   - Vercel will automatically detect it as a **Static Project** (no build settings are required).
   - Click **Deploy**.
4. **Access Your Portal**: Your app will be live at `https://<project-name>.vercel.app`.

### Option 2: Deploy via Vercel CLI (Quickest)
If you have the Vercel CLI installed locally, you can deploy it instantly from your terminal:
1. Install Vercel CLI (if not already installed):
   ```bash
   npm install -g vercel
   ```
2. Log in and deploy:
   ```bash
   vercel login
   vercel
   ```
3. Follow the interactive prompts. Once complete, your project will be deployed instantly!
