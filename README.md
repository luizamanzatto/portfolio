# Your Designer Portfolio

This repository contains the code for a simple, static HTML/CSS portfolio website designed to showcase your projects.

## Structure

- `index.html`: The main landing page with the project grid and sidebar navigation.
- `style.css`: Contains all the styling rules for the website.
- `projects/`: This directory holds the individual HTML pages for each project.
  - `project_template.html`: A template file to use as a starting point for new project pages.
  - `project1.html`, `project2.html`, ...: Individual project pages (copy and modify the template).
- `images/`: This directory should contain all your images:
  - Project cover images (used in the grid on `index.html`).
  - Detailed images and GIFs for individual project pages.

## How to Add a New Project

1.  **Prepare Images:**
    *   Create a cover image for the project grid (e.g., `projectX_cover.png`).
    *   Gather detailed images and GIFs for the project page (e.g., `projectX_detail1.png`, `projectX_animation.gif`).
    *   Place all these images inside the `images/` directory.

2.  **Create Project Page:**
    *   Duplicate the `projects/project_template.html` file.
    *   Rename the duplicate file to match your project (e.g., `projects/projectX.html`).
    *   Edit the new `projectX.html` file:
        *   Change the `<title>`.
        *   Update the `<h1>Project Title</h1>`.
        *   Fill in the Category and Project Summary.
        *   Replace the placeholder `<img>` tags with your actual project images from the `images/` directory. Remember to update the `src` and `alt` attributes.

3.  **Add to Main Page (`index.html`):**
    *   **Sidebar:** Add a new list item `<li>` to the navigation `<ul>` in the `<aside class="sidebar">` section, linking to your new project page:
        ```html
        <li><a href="projects/projectX.html">Project X Name</a></li>
        ```
    *   **Project Grid:** Add a new `<a class="project-box">` element within the `<main class="projects-grid">` section:
        ```html
        <a href="projects/projectX.html" class="project-box" id="projectX">
            <img src="images/projectX_cover.png" alt="Project X Cover">
            <div class="project-name">Project X Name</div>
        </a>
        ```
        Make sure the `href` points to your new HTML file and the `img src` points to your new cover image.

4.  **Save and Preview:** Save all your changes and open `index.html` in your web browser to see the updated portfolio.

## Customization

- **Styling:** Modify `style.css` to change colors, fonts, layout, and hover effects.
- **Content:** Replace all placeholder text and images with your own content.
- **Name:** Change "Your Name" in `index.html` and the project template. 