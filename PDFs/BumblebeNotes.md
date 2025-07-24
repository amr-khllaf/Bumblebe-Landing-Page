---
title: 3D Robot Website Using HTML & CSS and Spline Notes
date: 24 - July - 2025
---

# Nesting in SCSS (or Sass) Or CSS

- Like SCSS, CSS also supports nesting, We Can do this in css:

- index.html File

```html
<div class="container">
  <header>
    <h1 class="logo">Bumblebee</h1>
    <nav>
      <ul>
        <li>
          <a href="#">Home</a>
        </li>
        <li>
          <a href="#">About</a>
        </li>
        <li>
          <a href="#">Services</a>
        </li>
        <li>
          <a href="#">Contact</a>
        </li>
      </ul>
    </nav>
    <button class="btn-signing"></button>
  </header>
</div>
```

- style.css File

```css
nav {
  display: flex;
  align-items: center;
  z-index: 999;
  ul {
    display: flex;
    list-style: none;
    gap: 2rem;
  }

  li {
    margin: 0 1rem;
  }

  a {
    text-decoration: none;
    color: inherit;
  }
}
```

- In this example, the `nav` element contains an unordered list (`ul`), list items (`li`), and anchor tags (`a`). The styles for each element are nested within the parent element, making it easier to read and maintain.

- This is Equivalent to the following CSS:

```css
nav {
  display: flex;
  align-items: center;
  z-index: 999;
}
nav ul {
  display: flex;
  list-style: none;
  gap: 2rem;
}
nav li {
  margin: 0 1rem;
}
nav a {
  text-decoration: none;
  color: inherit;
}
```

---

# Introduction To Spline Tool

- Spline is a 3D design tool that allows you to create and share interactive 3D content on the web. It provides an intuitive interface for designing 3D models, animations, and scenes that can be embedded in websites.
- Spline supports various features such as real-time collaboration, animation, and interactivity, making it suitable for creating engaging 3D experiences.
- To use Spline, you can create a free account on their website and start designing your 3D models. Once your model is ready, you can export it and embed it in your HTML using an iframe or a script tag.

[Spline Website](https://spline.design/)

## Steps to Use Spline

1. **Create a Spline Account**: Go to the Spline website and sign up for a free account.
2. Go to the Community section and find the 3D model you want to use.
3. Click on the model to open it in the editor by clicking on remix Button.
4. **Customize the Model**: You can modify the model, add animations, and set up interactions as needed.
5. **Export the Model**: Once you're satisfied with your design, you can export it. Spline provides options to export your model as an iframe or a script tag.
6. Click on the Viewer button to get the embed code.
7. **Embed in HTML**: Copy the provided code and paste it into your HTML file where you want the 3D model to appear.

```html
<script
  type="module"
  src="https://unpkg.com/@splinetool/viewer@1.10.36/build/spline-viewer.js"
></script>
<spline-viewer
  url="https://prod.spline.design/CV8STXkT5-jmqY5w/scene.splinecode"
></spline-viewer>
```

- The Link is consist of 2 parts:
  - The first part is the script tag that loads the Spline viewer.
  - The second part is the `<spline-viewer>` tag that contains the URL of your Spline model.

---

# Using AOS (Animate On Scroll) Library

- AOS (Animate On Scroll) is a library that allows you to animate elements as they scroll into view. It provides a simple way to add animations to your web pages without writing custom JavaScript.

- To use AOS, you need to include the AOS CSS and JavaScript files in your HTML. You can either download them or link to a CDN.

```html
<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.css"
/>
```
