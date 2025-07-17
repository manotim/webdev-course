The page is divided into clear sections using semantic tags (<header>, <section>, <footer>). This improves readability, accessibility, and SEO.

<body>
  <header>...</header>        <!-- Company branding -->
  <section>...</section>      <!-- About us -->
  <section>...</section>      <!-- Featured cars (cards) -->
  <section>...</section>      <!-- Car comparison table -->
  <section>...</section>      <!-- Contact form -->
  <div class="fixed-box">...</div> <!-- Fixed button -->
  <footer>...</footer>        <!-- Footer links -->
</body>

🎨 2. CSS STYLE EXPLANATION (Line-by-Line Commentary)
✅ body Styling

body {
  font-family: Arial, sans-serif;
  background: linear-gradient(to right, #f5f7fa, #c3cfe2);
  margin: 0;
  padding: 0;
}
font-family: Clean sans-serif font.

background: Smooth gradient for a more modern look.

margin/padding: 0: Resets browser defaults (standard practice).

✅ header Section

header {
  background-color: #1e2a38;
  color: white;
  text-align: center;
  padding: 40px 20px;
}
Dark blue-gray background for contrast.

Text centered with padding to create white space.

Inside it, we use <h1> for branding, and <p> for tagline.

header img {
  width: 100px;
}
Logo image width set to a fixed size to prevent layout breaking.

✅ General Section Padding

section, .card-container, footer {
  padding: 20px;
}
Keeps consistent spacing around all page sections.

✅ Card Layout (Car Profiles)

.card-container {
  display: flex;
  gap: 20px;
  justify-content: space-around;
  flex-wrap: wrap;
}
display: flex: Aligns cards horizontally.

gap: Space between cards.

flex-wrap: wrap: Allows cards to stack on small screens.

.profile-card {
  background-color: white;
  border: 1px solid #ccc;
  border-radius: 12px;
  padding: 15px;
  width: 250px;
  position: relative;
  box-shadow: 2px 2px 10px rgba(0,0,0,0.1);
}
Card styling: white box with soft border and rounded corners.

position: relative: Allows positioning child elements (like .price-tag) absolutely within the card.

.price-tag {
  position: absolute;
  top: 10px;
  right: 10px;
  background: crimson;
  color: white;
  padding: 5px 10px;
  font-weight: bold;
  border-radius: 5px;
  z-index: 10;
}
Positioned on top-right of the card.

z-index: 10: Ensures it appears above the image.

✅ Car Table Styling

table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 20px;
}
Full-width table.

border-collapse: Combines adjacent borders into one clean line.




th, td {
  border: 1px solid #999;
  padding: 10px;
  text-align: center;
}

th {
  background-color: #333;
  color: white;
}
Clean bordered layout.

Header cells have dark background to separate from data.

✅ Contact Form Styling

form {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  max-width: 600px;
  margin: auto;
}
Makes form more readable and clean.

margin: auto: Center-aligns the form.

Rounded corners for a friendly look.

input, select, textarea {
  width: 100%;
  padding: 8px;
  margin-top: 5px;
  border: 1px solid #ccc;
  border-radius: 5px;
}
Uniform spacing, full width inputs for mobile-friendliness.

Rounded borders for modern design.

✅ Fixed Box (Sticky Button)

.fixed-box {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background-color: #333;
  color: white;
  padding: 10px 20px;
  border-radius: 8px;
  z-index: 999;
}
Sticks to the bottom-right corner of the screen.

z-index: 999 ensures it stays on top of all content.

Great for things like contact buttons, help chat, or "back to top".

✅ Footer Styling
css
footer {
  background-color: #1e2a38;
  color: white;
  text-align: center;
  padding: 20px;
}
Matches header for design consistency.

footer a {
  color: #ddd;
  text-decoration: none;
  margin: 0 10px;
}
Light gray links spaced nicely.