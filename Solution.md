Plaintext
assignment-5.1/
├── index.html
└── style.css
1. External Stylesheet (style.css)
CSS
/* 3. Body background, text color, and font */
body {
  margin: 0;
  padding: 0;
  background-color: #f1f5f9;
  color: #1e293b;
  font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  font-size: 16px;
  line-height: 1.65;
}

.container {
  max-width: 900px;
  margin: 0 auto;
  padding: 0 1.25rem;
}

/* Header & 5. Readable, attractive navigation links */
header {
  background-color: #0f172a;
  color: #ffffff;
  padding: 1rem 0;
  border-bottom: 3px solid #2563eb;
}

.nav-wrapper {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  gap: 1rem;
}

.logo {
  font-size: 1.3rem;
  font-weight: 700;
  color: #ffffff;
  text-decoration: none;
  letter-spacing: 0.3px;
}

nav ul {
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  gap: 0.6rem;
  margin: 0;
  padding: 0;
}

nav a {
  display: inline-block;
  color: #e2e8f0;
  background-color: #1e293b;
  text-decoration: none;
  font-weight: 600;
  padding: 0.45rem 0.9rem;
  border-radius: 6px;
  transition: background-color 0.2s ease, color 0.2s ease;
}

nav a:hover,
nav a:focus {
  background-color: #2563eb;
  color: #ffffff;
}

nav a.active {
  background-color: #2563eb;
  color: #ffffff;
}

/* Main Content Layout */
main {
  padding: 2rem 0 3rem;
}

section {
  background-color: #ffffff;
  border: 1px solid #cbd5e1;
  border-radius: 10px;
  padding: 1.75rem;
  margin-bottom: 1.5rem;
  box-shadow: 0 2px 8px rgba(15, 23, 42, 0.05);
}

/* 4. Style headings, paragraphs, and links */
h1 {
  color: #0f172a;
  font-size: 2rem;
  line-height: 1.25;
  margin-top: 0;
  margin-bottom: 0.75rem;
}

h2 {
  color: #1d4ed8;
  font-size: 1.35rem;
  margin-top: 0;
  margin-bottom: 0.6rem;
  border-bottom: 2px solid #e2e8f0;
  padding-bottom: 0.35rem;
}

p {
  color: #334155;
  margin-top: 0;
  margin-bottom: 1rem;
}

main a {
  color: #1d4ed8;
  font-weight: 600;
  text-decoration: underline;
  text-underline-offset: 3px;
}

main a:hover {
  color: #1e40af;
  background-color: #eff6ff;
}

.cta-button {
  display: inline-block;
  background-color: #2563eb;
  color: #ffffff;
  text-decoration: none;
  padding: 0.6rem 1.2rem;
  border-radius: 6px;
  margin-top: 0.25rem;
}

.cta-button:hover {
  background-color: #1d4ed8;
  color: #ffffff;
}

/* Footer */
footer {
  background-color: #0f172a;
  color: #cbd5e1;
  text-align: center;
  padding: 1.25rem 0;
  font-size: 0.9rem;
}

footer p {
  color: #cbd5e1;
  margin: 0;
}
2. Styled HTML Page (index.html)
HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ByteCraft Coding Club — Styled Home Page</title>
  <meta name="description" content="Styled home page for ByteCraft Coding Club using an external style.css stylesheet." />
  <!-- 2. Link the external stylesheet in HTML -->
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <div class="container nav-wrapper">
      <a class="logo" href="index.html">ByteCraft Club</a>
      <nav aria-label="Primary Navigation">
        <ul>
          <li><a class="active" href="index.html">Home</a></li>
          <li><a href="about.html">About</a></li>
          <li><a href="registration.html">Register</a></li>
          <li><a href="contact.html">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <main class="container">
    <section>
      <h1>Welcome to ByteCraft Coding Club</h1>
      <p>
        ByteCraft is our campus developer community where students collaborate on web projects,
        practice problem-solving, and host weekly hands-on coding sessions.
      </p>
      <p>
        New members of all skill levels are welcome. Explore our
        <a href="about.html">club leadership and history</a> or sign up directly for this semester's
        workshops.
      </p>
      <a class="cta-button" href="registration.html">Register Now</a>
    </section>

    <section>
      <h2>Weekly Activities</h2>
      <p>
        Every Thursday from 4:00 PM to 5:30 PM in CS Lab 204, we run guided build sessions covering
        HTML, CSS, Git, and JavaScript fundamentals.
      </p>
      <p>
        Have questions before joining? Visit our <a href="contact.html">contact page</a> or email us
        at <a href="mailto:bytecraft@college.edu">bytecraft@college.edu</a>.
      </p>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>&copy; 2026 ByteCraft Coding Club — Styled with external style.css</p>
    </div>
  </footer>
</body>
</html>