---
layout: default
title: MTE 481 FYDP Group 23
---

<style>
  body {
    font-family: 'Work Sans', sans-serif;
    margin: 0;
    background-color: #f4f4f4;
    color: #333;
  }

  header {
    background-color: #7b6f90;
    color: white;
    padding: 20px 0 10px;
    text-align: center;
  }

  header h1 {
    font-family: 'Oswald', sans-serif;
    font-size: 28px;
    margin: 0;
  }

  header p {
    margin: 4px 0 13px;
    font-size: 16px;
  }

  .container {
    padding: 20px;
    max-width: 900px;
    margin: auto;
  }

  h2 {
    font-family: 'Work Sans', sans-serif;
    border-bottom: 2px solid #004080;
    padding-bottom: 5px;
    margin-top: 30px;
  }

  ul {
    list-style-type: disc;
    padding-left: 20px;
  }

  ul li {
    margin-bottom: 10px;
  }

  ul li p {
    margin: 4px 0 10px;
    font-size: 0.9em;
    color: #555;
  }

  .copy-email {
    color: #004080;
    text-decoration: underline;
    cursor: pointer;
  }

  .copy-email:hover {
    color: #00264d;
  }

  footer {
    text-align: center;
    padding: 10px;
    background-color: #ddd;
    margin-top: 40px;
  }
</style>

<link href="https://fonts.googleapis.com/css2?family=Oswald:wght@400;600&family=Work+Sans:wght@400;500;600&display=swap" rel="stylesheet" />

<header>
  <h1>MTE 481 FYDP Group 23</h1>
  <p>Capstone Design Project Log</p>
</header>

<div class="container">

## Team Members

- **Francisco Jao** - Electrical  
  Email: <span class="copy-email" data-email="fmojao@uwaterloo.ca">fmojao@uwaterloo.ca</span>

- **Annie Lee** - Electrical  
  Email: <span class="copy-email" data-email="a363lee@uwaterloo.ca">a363lee@uwaterloo.ca</span>

- **Angadbir Singh** - Mechanical  
  Email: <span class="copy-email" data-email="a555sing@uwaterloo.ca">a555sing@uwaterloo.ca</span>

- **Larry Wu** - Mechanical  
  Email: <span class="copy-email" data-email="l233wu@uwaterloo.ca">l233wu@uwaterloo.ca</span>

- **Waris Zahoor** - Software  
  Email: <span class="copy-email" data-email="w2zahoor@uwaterloo.ca">w2zahoor@uwaterloo.ca</span>

## Project Description

Brief description of the capstone project. Section for objectives, goals, and current progress overview.

## Progress Logs

- [Week 2 - Sept 9, 2025](meetings/sept-9-2025.md)
- [Week 3 - Sept 10, 2025](meetings/sept-10-2025.md)
- [Week 4 - Sept 22, 2025](meetings/sept-22-2025.md)

</div>

<footer>
  &copy; 2025 Group 23 | MTE 481 | University of Waterloo
</footer>

<script>
  // Copy email functionality
  document.querySelectorAll('.copy-email').forEach(span => {
    span.title = 'Click to copy email';
    span.addEventListener('click', () => {
      const email = span.getAttribute('data-email');
      navigator.clipboard.writeText(email).then(() => {
        const originalText = email;
        span.textContent = originalText + ' (Copied!)';
        setTimeout(() => {
          span.textContent = originalText;
        }, 1500);
      }).catch(err => {
        console.error('Failed to copy email: ', err);
      });
    });
  });
</script>