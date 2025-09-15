# **Animated HTML Resume & GitHub Pages Hosting**

This repository contains an animated HTML/CSS resume template. Below are the combined instructions for customizing the template with your information and publishing it as a live website using GitHub Pages.

See the Template here for example ->  https://ee-edk.github.io/Career-Resume-Template-HTML-Website/

## **Section 1: How to Customize Your Resume Template**

You must replace all placeholder text marked with \[brackets\] with your own information.

### **Step-by-Step Customization**

1. **Header:** Locate the \<header class="header"\> section. Update placeholders for your name, professional title, location, phone, email, and LinkedIn URL.  
2. **Professional Summary:** Find the \<div class="summary-content"\>. Write 3-4 compelling sentences about yourself, making sure to include your years of experience and key achievements (using numbers when possible).  
3. **Core Competencies:** In the competencies-grid section, replace the four \[Skill Category X\] headings with your main skill areas (e.g., Technical Skills, Leadership, Project Management). List 4-5 specific skills under each category.  
4. **Professional Experience:**  
   * Update your job information, including \[Company Name\], \[Your Job Title\], and employment dates (e.g., "Jan 2020 \- Dec 2023").  
   * Replace each \[Achievement description\] with specific accomplishments. Use action verbs (like Led, Managed, or Increased) and include numbers or percentages whenever you can.  
5. **Education:** In the education-grid section, update your \[Degree Name\], school name, and location.  
6. **Technical Expertise:** Find the tech-grid section. Update the \[Skill Category\] (e.g., "Programming Languages") and list specific skills. Update the percentage (XX%) to reflect your comfort level (e.g., 70-80% for proficient, 90-95% for expert).

### **Adding or Removing Sections**

* **To Add More Jobs:** Copy an entire \<div class="experience-item"\> block and paste it below the existing one. Then, fill in the new job details. Use the same method for adding more degrees.  
* **To Remove Sections:** To delete optional sections like "Military Service" or "Honors & Awards", find the section starting with \<section class="section" and delete everything from that opening tag to its matching closing \</section\> tag.

### **Saving Your File**

When you are finished customizing, save the file as resume.html. You can open this file in any web browser to see your changes and use the "Download PDF" button to print or save a PDF version.

**Important:** For the next steps (hosting), you will need to **rename this file.**

## **Section 2: How to Host Your Resume on GitHub Pages**

Follow these steps to publish your newly customized resume as a live website.

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
