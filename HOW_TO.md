# How to Customize Your Professional Resume Template

This guide provides step-by-step instructions on how to personalize your animated HTML resume.

## Table of Contents
1.  [Getting Started](#getting-started)
2.  [Editing Content](#editing-content)
    - [Header & Contact Info](#header--contact-info)
    - [Professional Summary](#professional-summary)
    - [Core Competencies](#core-competencies)
    - [Professional Experience](#professional-experience)
    - [Education](#education)
    - [Technical Expertise](#technical-expertise)
3.  [Using Optional Sections](#using-optional-sections)
    - [Enabling a Section](#enabling-a-section)
    - [Key Projects](#key-projects)
    - [Military Service](#military-service)
    - [Honors & Awards](#honors--awards)
    - [Publications](#publications)
    - [Languages](#languages)
4.  [Customizing Appearance](#customizing-appearance)
    - [Changing the Theme Color](#changing-the-theme-color)
    - [Adding a Headshot or Logo](#adding-a-headshot-or-logo)
5.  [Saving and Viewing](#saving-and-viewing)

---

## Getting Started

To edit the template, you need a code editor (like [VS Code](https://code.visualstudio.com/), [Sublime Text](https://www.sublimetext.com/), or even a basic text editor like Notepad).

Open the `index.html` file in your editor to begin making changes. All the content and styling are in this single file.

## Editing Content

All the text you need to change is marked with `[square brackets]` and is usually preceded by a comment like `<!-- CHANGE THIS -->`.

### Header & Contact Info

1.  **Title:** In the `<head>` section at the top of the file, find `<title>[YOUR NAME] - [YOUR PROFESSION/TITLE]</title>` and update it. This is what appears in the browser tab.
2.  **Name & Title:** In the `<body>`, find the `<header>` section. Replace `[YOUR FULL NAME]` and `[Your Professional Title] | [Your Industry/Specialty]`.
3.  **Contact Information:** Locate the `<div class="contact-info">`.
    *   Replace the bracketed text with your email, phone number, location, portfolio, and LinkedIn profile URL.
    *   The links are already set up. For email, change `[your.email@example.com]` in `href="mailto:[your.email@example.com]"`. Do the same for your phone number in `href="tel:[Your Phone Number]"`.
    *   **For Developers:** You can uncomment the GitHub link and add your profile.

### Professional Summary

Find the section with the title `Professional Summary`. Inside the `<div class="summary-content">`, replace the placeholder paragraph with a compelling 2-4 sentence summary of your career, skills, and goals. The comments provide a helpful example.

### Core Competencies

Under the `Core Competencies` title, you'll find several `<div class="competency-group">` blocks.
1.  Change the `<h4>` heading to a relevant skill category (e.g., "Data Analysis," "Software Development").
2.  Update the list items `<li>` with your specific skills or tools for that category.

### Professional Experience

This is a critical section. For each job you've held, there is an `<div class="experience-item">` block.
1.  Update the `[Company Name]`, `[City, State]`, `[Your Job Title]`, and employment dates.
2.  In the `<ul class="achievements">`, list your key accomplishments.
    *   **Be specific:** Use strong action verbs (e.g., *Managed*, *Developed*, *Increased*).
    *   **Quantify your results:** Use numbers, percentages, or dollar amounts to show your impact (e.g., "Increased team productivity by 25%").
3.  **To add more jobs:** Copy an entire `<div class="experience-item">...</div>` block and paste it below the last one. Fill in the new details.

### Education

In the `Education` section, update the `<div class="education-item">` blocks with your degree, university, and any honors. You can also use this for certifications.

### Technical Expertise

In the `Technical Expertise` section:
1.  Update the `<h4>` with a skill category (e.g., "Programming Languages," "Databases").
2.  For each skill, update the `<span class="skill-name">` and set your proficiency level in the `data-level` attribute (e.g., `data-level="90%"`). This percentage controls the width of the animated skill bar.

---

## Using Optional Sections

The template includes several optional sections that are **commented out** by default. This means they are present in the code but are not visible in the browser.

### Enabling a Section

To make an optional section appear on your resume, you need to remove the comment tags surrounding it.
- Find the start of the section, which looks like: `<!-- OPTIONAL SECTION: [SECTION NAME]...`
- Delete the `<!--` from the beginning and the `-->` from the end of the section block.

The available optional sections are:
-   **Key Projects:** Ideal for showing off your work with links.
-   **Military Service:** A dedicated format for military experience.
-   **Honors & Awards:** List your professional or academic awards.
-   **Publications:** For academics and researchers.
-   **Languages:** List the languages you speak and your proficiency.

---

## Customizing Appearance

### Changing the Theme Color

You can easily change the main accent color of the resume (the red color used for links, bullets, etc.).
1.  In the header, click the paintbrush icon (`🎨`).
2.  A palette of pre-selected colors will appear.
3.  Click any color to instantly change the theme. Your choice is automatically saved in your browser for the next time you visit.

### Adding a Headshot or Logo

You can add a small image to the header (like a professional headshot).
1.  Find the line: `<!-- OPTIONAL: Add a professional headshot or company logo... -->`
2.  Uncomment the `<img>` tag by removing the `<!--` and `-->`.
3.  Replace `"your-logo.jpg"` with the path to your image file. Make sure the image file is in the same folder as your `index.html` file, or provide the correct path.
4.  A recommended size is around 150x150 pixels.

---

## Saving and Viewing

After making your changes, save the `index.html` file. You can open it directly in a web browser (like Chrome, Firefox, or Safari) to see your live, animated resume.

To create a PDF version, use the "Download PDF" button, which will open your browser's print dialog. From there, you can choose to "Save as PDF".
