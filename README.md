# Interactive JSON-Powered Resume

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Made with: HTML, CSS, JS](https://img.shields.io/badge/Made%20with-HTML%2C%20CSS%2C%20JS-orange.svg)](https://developer.mozilla.org/)
[![GitHub Stars](https://img.shields.io/github/stars/adnaanaeem/adnaanaeem.github.io?style=social)](https://github.com/adnaanaeem/adnaanaeem.github.io/stargazers)

A simple, modern, and feature-rich online resume template that is dynamically powered by a single `resume.json` file. Perfect for developers who want a professional online presence without the hassle of frameworks or build tools.

### [View the Live Demo](https://adnaanaeem.github.io/)

![Live Resume Screenshot](social_card.png)
*(This project uses the `social_card.png` as its preview image. You should create your own!)*

---

## ✨ Key Features

*   **Single Source of Truth**: All resume data is managed in one clean `data.json` file. No need to edit HTML!
*   **Fully Responsive**: Looks great on desktop, tablet, and mobile devices.
*   **Dark Mode**: A sleek, modern dark theme that can be toggled by the user.
*   **Interactive Menu**: A Floating Action Button (FAB) provides easy access to all features.
*   **Download as PDF**: Generate and download a pixel-perfect PDF of the resume.
*   **ATS-Friendly Mode**: Toggle the profile picture off for a clean, Applicant Tracking System (ATS) optimized layout.
*   **SEO & Social Sharing Ready**: Includes all necessary meta tags for great search engine results and rich link previews on social media.
*   **Zero Dependencies**: Built with pure HTML, CSS, and JavaScript. No frameworks, no build steps.

## 🚀 Getting Started

Follow these simple steps to set up your own personal resume.

### Step 1: Fork the Repository

Click the "Fork" button at the top-right of this page to copy this project to your own GitHub account.

### Step 2: Customize Your Information (`data.json`)

This is where you'll spend most of your time. Open the `data.json` file and edit the content to reflect your personal information. The structure is straightforward:

*   **`meta`**: Contains all data for SEO and social sharing cards. Update the titles, descriptions, and URLs here.
*   **`name`, `title`**: Your full name and professional title.
*   **`contact`**: Your contact details.
*   **`sectionOrder`**: **Important!** This array controls the order of the sections on your resume. You can re-arrange or remove sections by editing this list.
*   **`summary`, `experience`, `skills`, `projects`, `education`**: These sections contain the main content of your resume. Follow the existing structure to add your own items.

```json
{
  "meta": {
    "title": "Your Name - Your Title",
    "description": "A brief, compelling description of you for search engines.",
    "social": {
      "ogTitle": "Your Name - Your Title",
      "ogDescription": "A slightly different description for social media previews.",
      "imageUrl": "https://yourusername.github.io/social_card.png"
      // ... and other social details
    }
  },
  "name": "Your Name",
  "title": "Your Professional Title",
  "contact": {
    "email": "your.email@example.com",
    "phone": "+123456789",
    "website": "https://yourportfolio.com",
    "linkedin": "https://linkedin.com/in/yourprofile"
  },
  "sectionOrder": [
    "summary",
    "experience",
    "skills",
    "projects",
    "education"
  ],
  "experience": [
    {
      "company": "Some Company",
      "title": "Your Role",
      "dates": "Jan 2020 - Present",
      "location": "City, Country",
      "responsibilities": [
        "Accomplishment #1 (Quantify your results!)",
        "Accomplishment #2"
      ]
    }
  ],
  // ... and so on for the other sections
}