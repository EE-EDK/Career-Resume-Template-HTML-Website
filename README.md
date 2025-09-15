# **Professional & Animated HTML Resume Template**

This repository contains a professional, animated, and highly customizable HTML resume template. It is designed to be a single `index.html` file that you can easily edit and host for free using GitHub Pages.

**Live Demo:** [Click here to see the template in action](https://ee-edk.github.io/Career-Resume-Template-HTML-Website/)

## **Features**

*   **Modern Design:** A clean, professional layout that looks great on all devices.
*   **Smooth Animations:** Subtle animations that engage visitors as they scroll.
*   **Themeable:** Easily change the accent color to match your personal brand with the built-in theme switcher.
*   **Highly Customizable:** Includes optional sections for projects, publications, languages, and more.
*   **Print-Friendly:** Prints a clean, professional-looking PDF version of your resume.

---

## **How to Use This Template**

There are two main parts to using this template: customizing it with your information and publishing it online.

### **1. Customizing Your Resume**

All the instructions for editing the content, enabling optional sections, and changing the appearance are in the detailed guide below:

**➡️ [Click here for the full Customization Guide](./HOW_TO.md)**

### **2. Hosting on GitHub Pages**

Once your resume is customized, follow these steps to publish it as a live website.

### **Step 1: Sign Up for GitHub**

You need a GitHub account. Go to github.com, click "Sign up", and follow the instructions to create your account. The username you choose will be part of your website's final address. When finished, make sure to verify your email address by clicking the link they send you.

### **Step 2: Install Git**

You must install the Git program to "talk" to GitHub from your computer.

1. Go to the official download page: git-scm.com/downloads.  
2. The site should automatically detect if you are on Windows or a Mac and show the correct download button. Click it to download the installer.  
3. Run the installer. It will ask many confusing questions. Just **accept all the default settings**. Keep clicking "Next" until it finishes. You do not need to change any settings.

### **Step 3: Prepare Your Project Folder**

1. Create a new folder on your computer. The Desktop is a good place. Name this folder my-first-website.  
2. **Crucial Step:** For GitHub Pages to work, your main HTML file **must be named index.html**. Find your customized resume.html file (from Section 1\) and **rename it to index.html**.  
3. Move your newly named index.html file into the my-first-website folder.

### **Step 4: Create a Local Repository (Command Line)**

1. Open your command-line tool.  
   * **On Windows:** Open the Start Menu, type Git Bash, and click the "Git Bash" application.  
   * **On Mac:** Open "Applications," then "Utilities," and open the "Terminal" app.  
2. Navigate to the folder you created using the cd (change directory) command. Since it's on the Desktop, the command is:  
   cd Desktop/my-first-website

   (Type this and press Enter).  
3. Type the following command to turn this folder into a Git repository:  
   git init

   (Press Enter. This creates a hidden .git subfolder where tracking information is stored).  
4. Tell Git to add all files in the folder to the tracking "staging area":  
   git add .

   (The . means "all files" in this directory. Press Enter).  
5. Save a "snapshot" (a "commit") of your project. We add a message (-m) to describe what we did:  
   git commit \-m "Initial commit: Add index.html"

   (Type this and press Enter).

### **Step 5: Create a Repository on GitHub**

Now that the project is saved on your computer, we need an empty repository on the GitHub website to hold it.

1. Go to your GitHub account in your browser.  
2. In the top-right corner, click the **\+** icon and select **"New repository"**.  
3. Fill out the form:  
   * **Repository name:** Give it the exact same name as your folder: my-first-website.  
   * **IMPORTANT:** You must select **"Public"**. GitHub Pages does not work with private repositories on the free plan.  
   * **Do NOT** check the boxes for "Add a README file," "Add .gitignore," or "Choose a license". We already have our project, and we don't want GitHub adding extra files.  
4. Click the green "Create repository" button.

### **Step 6: Push Your Code to GitHub**

GitHub will now show you a page with commands under the heading "...or push an existing repository from the command line".

1. Go back to your command-line window (Git Bash or Terminal).  
2. Copy the lines from the GitHub page and paste them into your terminal, one by one, pressing Enter after each one. They will look exactly like this (but with *your* username instead of your-username):  
   git remote add origin \[https://github.com/your-username/my-first-website.git\](https://github.com/your-username/my-first-website.git)  
   git branch \-M main  
   git push \-u origin main

3. When you run the git push command, a browser window may pop up asking you to sign in or authorize the connection. Approve it.  
4. After the push finishes, refresh your repository page on GitHub. You should now see your index.html file listed there.

### **Step 7: Activate GitHub Pages and Go Live\!**

This is the final step to turn your repository into a live website.

1. On your GitHub repository page, click the **"Settings"** tab (it has a gear icon).  
2. In the sidebar on the left, click **"Pages"**.  
3. Under the "Build and deployment" section, find "Source". It should say "Deploy from a branch".  
4. In the dropdown menu under that section, select the branch named **main**.  
5. Click **"Save"**.  
6. The page will refresh. It might take a minute or two for the site to be ready. Refresh the page again until you see a green box at the top with your URL.

Congratulations\! Your site is live at the following URL:  
https://your-username.github.io/my-first-website/
