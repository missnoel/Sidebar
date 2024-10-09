
# Sidebar Project
This project demonstrates how to create a responsive sidebar using HTML, CSS, and JavaScript. The sidebar can be toggled (shown or hidden) with a button click and provides navigation links, social media icons, and a logo. Users can open the sidebar by clicking the hamburger icon and close it by clicking the close button.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [How It Works](#how-it-works)
- [Project Structure](#project-structure)

## Overview
The sidebar project is a simple yet functional example of how to create a collapsible sidebar for website navigation. The project leverages basic HTML for structure, CSS for styling, and JavaScript for interactivity. It can be extended and modified based on specific design or functionality requirements.

## Features
- Responsive Design: The sidebar adjusts its behavior based on the screen size, making it mobile-friendly.
- Toggle Button: A hamburger button is used to open and close the sidebar.
- Close Button: The sidebar contains a close button for user convenience.
- Navigation Links: Includes links to various pages (home, about, projects, contact).
- Social Media Icons: Displays social media icons using Font Awesome for easy navigation to social profiles.

## Technologies Used
- HTML: Defines the structure of the page and sidebar.
- CSS: Provides layout and style for the sidebar, including fonts, colors, and responsive behaviors.
- JavaScript: Handles the interactive features such as opening and closing the sidebar.

## How It Works
*JavaScript*
- Opening the Sidebar: When the user clicks the toggle button (.sidebar-toggle), the JavaScript adds the class show-sidebar to the sidebar, making it visible.
- Closing the Sidebar: When the user clicks the close button (.close-btn), the JavaScript removes the show-sidebar class, hiding the sidebar again.

`javascript

// Selecting necessary DOM elements
const toggleBtn = document.querySelector('.sidebar-toggle');
const closeBtn = document.querySelector('.close-btn');
const sidebar = document.querySelector('.sidebar');

// Toggle the sidebar visibility when the hamburger button is clicked
toggleBtn.addEventListener('click', function() {
    sidebar.classList.toggle('show-sidebar');
});

// Close the sidebar when the close button is clicked
closeBtn.addEventListener('click', function() {
    sidebar.classList.remove('show-sidebar');
});`

CSS
The show-sidebar class is responsible for making the sidebar visible or hidden, with CSS transitions to animate the sidebar’s appearance.

`css

/* Sidebar is initially hidden */
.sidebar {
  transform: translateX(-100%);
  transition: transform 0.3s ease;
}

/* Sidebar appears when the class 'show-sidebar' is added */
.sidebar.show-sidebar {
  transform: translateX(0);
}`

/* Rest of the styling for layout and responsiveness */
Project Structure


├── index.html         # Main HTML file
├── styles.css         # CSS for styling the page
├── app.js             # JavaScript for sidebar functionality
├── logo.svg           # Logo image displayed in the sidebar

