# Photo Studio - HTML/CSS Sidebar Project

This is a simple, non-responsive project for a "Photo Studio" website, focusing on creating a sleek, slide-out sidebar menu using only HTML and CSS.

This project was built as part of a web development tutorial under the guidance of **Shradha Khapra (Apna College)**.

---

### 🚀 Live Demo

You can view the live deployed project here:
**[Click here to view the live project!](https://junaidusmani2468.github.io/Photo-Studio/)**

---

## 📸 Preview

![Photo Studio Preview](./assets/Photo-Studio-SS.png)

## 🚀 Features

* **Clean UI:** A modern, dark-theme design for a photography portfolio.
* **Pure CSS Sidebar:** The sidebar menu slides in and out using a "hidden checkbox" trick, requiring no JavaScript.
* **Font Awesome Icons:** Uses Font Awesome for clean, scalable icons.
* **Smooth Transitions:** CSS transitions are used for all hover effects and the main sidebar movement.

## 🛠️ Technologies Used

* **HTML5**
* **CSS3**
* **Font Awesome** (for icons)

## 😂 A Note on the "Creative" CSS!

As a fun learning note, this project includes an interesting bug that serves as a great lesson in CSS selectors.

* **The Goal:** When the "menu" (bars) icon is clicked, the sidebar should slide out, the "menu" icon should disappear, and a "close" (X) icon should appear.
* **The Bug:** The sidebar slides out correctly using the `:checked` pseudo-class and the general sibling combinator (`~`):
    `#check:checked ~ .sidebar_menu { left: 0; }`
* **The Problem:** The CSS rules to toggle the icons (`#check:checked ~ .btn_one`) do not work. This is because the icons (`.btn_one`, `.btn_two`) are not *siblings* of the `#check` input. They are *nested inside* the `label` elements, which are the actual siblings.
* **The Result:** The menu slides, but the icons don't toggle! This repository is a great example of how CSS selectors work and the importance of understanding the DOM structure.
