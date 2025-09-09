# charity-water-landing
A simple landing page for Charity: Water built with HTML and CSS.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Charity Water Landing Page</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- HERO SECTION -->
  <header class="hero">
    <h1>CHARITY WATER</h1>
    <p class="subhead">SEE WHERE YOUR DONATIONS GO. KNOW WHO YOU HELP</p>
    <p class="author">JOSH CASTOR <br> 09/125</p>
    <img src="img/hero.jpg" alt="Child with clean water" class="hero-image">
  </header>

  <!-- CONTENT SECTION -->
  <section class="content">
    <div class="column">
      <h2>CUSTOMER PERSONA</h2>
      <p><strong>Impact-Driven Millennial Maddie</strong><br>
         Age: 28<br>
         Occupation: Tech Company designer</p>
    </div>

    <div class="column">
      <h2>SIGNIFICANCE OF PHOTO?</h2>
      <p>This powerful image captures pure joy and hope in the eyes of a child who now has access to clean water. It visually communicates the life-changing impact of safe water, making it a compelling and emotional centerpiece for a Water Step flyer. The vibrant colors and genuine smile create an instant connection, inspiring viewers to take action.</p>
    </div>
  </section>

  <!-- VALUE PROPOSITION -->
  <section class="value">
    <h2>VALUE PROPOSITION</h2>
    <p>For socially conscious millennials who want full transparency and real impact, charity: water offers 100% direct to project giving, GPS tracked results, and immersive stories from the field unlike many traditional charities who blur where donations go.</p>
  
    <!-- Call to Action Button -->
    <a href="#" class="cta-button">Donate Now</a>
  </section>

  <!-- FOOTER -->
  <footer>
    <img src="img/logo.png" alt="Charity Water Logo" class="footer-logo">
  </footer>
</body>
</html>
/* General Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  color: #333;
  background-color: #fff;
}

/* HERO */
.hero {
  text-align: center;
  padding: 2rem;
}

.hero h1 {
  font-size: 2.5rem;
  color: #5a7ea1; /* blue-gray like in Canva mockup */
  margin-bottom: 0.5rem;
}

.subhead {
  font-size: 1rem;
  color: #7d8ea5;
  margin-bottom: 0.5rem;
}

.author {
  font-size: 0.9rem;
  color: #7d8ea5;
  margin-bottom: 1rem;
}

.hero-image {
  width: 100%;
  max-width: 900px;
  border-radius: 8px;
  margin-top: 1rem;
}

/* CONTENT */
.content {
  display: flex;
  flex-wrap: wrap;
  padding: 2rem;
  gap: 2rem;
}

.content .column {
  flex: 1;
  min-width: 280px;
}

.content h2 {
  font-size: 1.2rem;
  color: #5a7ea1;
  margin-bottom: 0.5rem;
}

/* VALUE PROPOSITION */
.value {
  padding: 2rem;
  background: #f6f9fc;
}

.value h2 {
  font-size: 1.2rem;
  color: #5a7ea1;
  margin-bottom: 1rem;
}

/* CTA BUTTON */
.cta-button {
  display: inline-block;
  margin-top: 1.5rem;
  padding: 0.8rem 2rem;
  font-size: 1rem;
  font-weight: bold;
  text-decoration: none;
  background-color: #f9c74f; /* vibrant yellow, matches charity: water theme */
  color: #000;
  border-radius: 30px;
  transition: background-color 0.3s ease, transform 0.2s ease;
}

.cta-button:hover {
  background-color: #f8961e; /* orange shade */
  transform: scale(1.05);
}

/* FOOTER */
footer {
  text-align: center;
  padding: 1.5rem;
}

.footer-logo {
  height: 50px;
}

/* ============================= */
/* RESPONSIVE DESIGN */
/* ============================= */

/* For tablets (max-width 768px) */
@media (max-width: 768px) {
  .hero h1 {
    font-size: 2rem;
  }

  .content {
    flex-direction: column;
    text-align: center;
  }
}

/* For mobile phones (max-width 480px) */
@media (max-width: 480px) {
  .hero {
    padding: 1rem;
  }

  .hero h1 {
    font-size: 1.6rem;
  }

  .subhead {
    font-size: 0.9rem;
  }

  .author {
    font-size: 0.8rem;
  }

  .value {
    padding: 1rem;
  }

  .value h2 {
    font-size: 1rem;
  }
}
