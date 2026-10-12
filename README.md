index.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>My Personal Website</title>
<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.6;
    background-color: #f4f4f4;
  }

header {
    background-color: #333;
    color: #fff;
    padding: 20px 0;
    text-align: center;
}

nav {
    margin-top: 10px;
}

nav a {
    color: #fff;
    margin: 0 15px;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    text-decoration: underline;
}

section {
    padding: 40px 20px;
    max-width: 800px;
    margin: 0 auto;
}

#about {
    background-color: #fff;
    margin-top: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

#contact {
    background-color: #f9f9f9;
    margin-top: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

form {
    display: flex;
    flex-direction: column;
}

label {
    margin-top: 10px;
    font-weight: bold;
}

input, textarea {
    padding: 10px;
    margin-top: 5px;
    border: 1px solid #ccc;
    border-radius: 4px;
    resize: vertical;
}

button {
    margin-top: 15px;
    padding: 10px 20px;
    background-color: #333;
    color: #fff;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: #555;
}

#status {
    margin-top: 10px;
    color: green;
}

.social {
    margin-top: 20px;
    display: flex;
    justify-content: center;
    gap: 20px;
}

.social a img {
    width: 40px;
    height: 40px;
    transition: transform 0.2s;
}

.social a img:hover {
    transform: scale(1.2);
}
</style>
</head>
<body>

<header>
  <h1>My Personal Website</h1>
  <nav>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section id="about">
  <h2>About Me</h2>
  <p>Hello! I'm [Your Name], a passionate developer with interests in web development, programming, and technology. Welcome to my personal website!</p>
</section>

<section id="contact">
  <h2>Contact Me</h2>
  <form id="contactForm">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required />

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required />

    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="5" required></textarea>

    <button type="submit">Send</button>
    <div id="status"></div>
  </form>
</section>

<section class="social">
  <a href="https://t.me/YourTelegramUsername" target="_blank" title="Telegram">
    <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/telegram.svg" alt="Telegram" />
  </a>
  <a href="https://github.com/YourGitHubUsername" target="_blank" title="GitHub">
    <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/github.svg" alt="GitHub" />
  </a>
  <a href="https://linkedin.com/in/YourLinkedInProfile" target="_blank" title="LinkedIn">
    <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/linkedin.svg" alt="LinkedIn" />
  </a>
</section>

<script>
  // Handle contact form submission
  document.getElementById('contactForm').addEventListener('submit', function(e) {
    e.preventDefault();

    // Optionally, you can process form data here
    const name = document.getElementById('name').value.trim();
    const email = document.getElementById('email').value.trim();
    const message = document.getElementById('message').value.trim();

    // Simple validation (HTML5 validation is already in place)
    if (!name || !email || !message) {
      alert('Please fill out all fields.');
      return;
    }

    // Show success message
    const statusDiv = document.getElementById('status');
    statusDiv.textContent = 'Your message has been sent!';
    statusDiv.style.color = 'green';

    // Reset form
    document.getElementById('contactForm').reset();
  });
</script>

</body>
</html>
```

### How to get your code:
- Copy all the above code.
- Paste it into a new file on your computer.
- Save the file with the name `index.html`.

### To customize:
- Replace `[Your Name]` with your actual name.
- Update the social links (`href`) with your actual profiles.
- Change the Telegram, GitHub, LinkedIn URLs accordingly.

Once saved, open `index.html` with your web browser to see your website locally. If you'd like, I can guide you through publishing it online—just ask!