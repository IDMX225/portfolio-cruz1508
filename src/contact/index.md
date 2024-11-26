---
layout: base.njk
title: Contact
---
<style>
  
  form {
    background-color: #f9f9f9;
    border-radius: 8px;
    box-shadow: 0 4px 9px rgba(0, 0, 0, 0.1);
    padding: 2em;
    max-width: 500px;
    margin: 0 auto;
    font-family: "Nunito", serif;
    color: #333;

  }
  h2 {
    font-family: 'Montserrat', sans-serif;
    font-size: 1.75rem;
    font-weight: 500;
    color: #508D4E;
    margin-bottom: 1.5em;
    text-align: center; 
  }

  
  input,
  textarea {
    font-family: inherit;
    font-size: 1rem;
    width: 100%;
    padding: 0.5em;
    margin-bottom: 1.5em;
    border: 1px solid black;
    border-radius: 1px;
    transition: border-color 0.3s ease;
  }

  label {
    font-weight: 600;
    margin-bottom: 0.5em;
    color: #508D4E;
  }

  textarea {
    height: 100px;
    resize: vertical;
  }

  button[type="submit"] {
    font-size: 1rem;
    padding: 1em;
    background-color: #508D4E;
    color: #ffff;
    width: 100%;
  }

 

  @media (max-width: 800px) {
    form {
      padding: 1em;
    }
  }
</style>

<h2>Contact Us</h2>

<form name="contact" method="POST" data-netlify="true">
  <p>
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
  </p>
  <p>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
  </p>
  <p>
    <label for="message">Message:</label>
    <textarea id="message" name="message" required></textarea>
  </p>
  <p>
    <button type="submit">Send</button>
  </p>
</form>