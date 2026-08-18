/* ================= HEADER LOGO + TITLE ================= */
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
}
header {
    background-color: #eee18a !important;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 25px;
    box-sizing: border-box;
}
header .logo {
    width: 100px;
    height: auto;
    margin-bottom: 10px;
}
header h1 {
    margin: 0;
    color: #000000;
    font-size: 36px;
    font-weight: bold;
}
/* Fixed Back to Top button floating on the bottom right */
.back-top {
    position: fixed;
    bottom: 20px;
    right: 20px;
    z-index: 1000;
    margin: 0;
}

.back-top a {
    background-color: #333;
    color: #fff;
    padding: 10px 15px;
    border-radius: 4px;
    text-decoration: none;
    box-shadow: 0 2px 5px rgba(0,0,0,0.3);
}

.back-top a:hover {
    background-color: #555;
}

/* ================= NAVIGATION ================= */

nav {
    background-color: #0fa8db;
    width: 100%;
}
nav ul {
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
    padding: 0;
    margin: 0;
}
nav li {
    margin: 0;
}
nav a {
    display: block;
    color: white;
    font-size: 18px;
    font-weight: bold;
    text-decoration: none;
    padding: 15px 20px;
}
nav a:hover,
nav a.active {
    background-color: #d4af37;
    color: black;
}

/* SLIDESHOW */
.slider {
width:80%;
max-width:900px;
height:450px;
margin:30px auto;
overflow:hidden;
position:relative;
}

.slider img {
position:absolute;
width:100%;
height:100%;
object-fit:cover;
opacity:0;
animation:fade 16s infinite;
}
.slider img:nth-child(1){
animation-delay:0s;
}
.slider img:nth-child(2){
animation-delay:4s;
}
.slider img:nth-child(3){
animation-delay:8s;
}
.slider img:nth-child(4){
animation-delay:12s;
}
@keyframes fade {
0%{
opacity:0;
}
5%{
opacity:1;
}
20%{
opacity:1;
}
25%{
opacity:0;
}
100%{
opacity:0;
}
}

/* CONTENT */

h2 {
text-align:center;
font-weight:bold;
font-size:32px;
}
.welcome-text {
font-family:"Times New Roman", serif;
text-align:left;
font-size:18px;
line-height:1.8;

}
.hours h3 {
    text-align: center;
    font-weight: bold;
}
.button {
display:block;
width:220px;
margin:30px auto;
text-align:center;
background:#d4af37;
color:black;
font-weight:bold;
padding:15px;
text-decoration:none;
border-radius:8px;
}
.button:hover {
background:#9f7a26;
color:rgb(111, 135, 49);

}
.hours {
text-align:center;
}
.hours h3 {
font-weight:bold;
font-size:24px;

}
/* ================= OPENING HOURS ================= */

.hours {
    text-align: center;
}

.hours h3 {
    text-align: center;
    font-size: 24px;
    font-weight: bold;
}

.hours p {
    text-align: center;
    font-size: 18px;
}
.social {
    margin-top: 20px;
    display: flex;
    justify-content: center;
    gap: 15px;
}

.social img {
    width: 40px;
    height: 40px;
    object-fit: contain;
    transition: transform 0.3s;
}

.social img:hover {
    transform: scale(1.2);
}
/* MOBILE */
@media(max-width:768px){
nav ul {
flex-direction:column;
}
.slider {
width:95%;
height:300px;
}
header h1 {
font-size:25px;
}
}
/* ================= FOOTER ================= */

footer {
    background-color: #eee18a;
    color: #000000;
    text-align: center;
    padding: 40px 20px; /* Keep vertical padding, adjust horizontal as needed */
    margin: 0;          /* Removes the 40px top/bottom and 20px side margins */
    width: 100%;        /* Forces it to take up the full width */
    box-sizing: border-box; /* Ensures padding doesn't push it past 100% width */
}
footer h3 {
    color: #000000;
    font-size: 26px;
    font-weight: bold;
}

footer p {
    color: #000000;
}

footer a {
    color: #000000;
    font-weight: bold;
    text-decoration: none;
    margin: 10px;
}

footer a:hover {
    color: #ffffff;
    text-decoration: underline;
}






/* --- Global Styling & Typography --- */
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: #333333;
    line-height: 1.6;
    background-color: #f9f9f9;
    margin: 0;
    padding: 0;
}

h1, h2, h3 {
    font-family: 'Georgia', serif;
    color: #2c3e50;
}

/* --- Menu Layout & Centering --- */
.menu-container {
    max-width: 900px;
    margin: 40px auto;
    background: #ffffff;
    padding: 40px;
    border-radius: 12px;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.05);
}

.menu-page-header h2, 
.menu-section > h2 {
    text-align: center;
    font-size: 2rem;
    margin-bottom: 30px;
    color: #1b4d3e; /* Deep Cedar Green flavor */
}

/* --- Menu Grid Item Layout --- */
.menu-list {
    display: flex;
    flex-direction: column;
    gap: 25px;
}

.menu-item {
    display: flex;
    align-items: center;
    gap: 20px;
    padding-bottom: 20px;
    border-bottom: 1px solid #eaeaea;
}

.menu-item:last-child {
    border-bottom: none;
}

/* --- Professional Image Sizing & Centering --- */
.menu-item img {
    width: 120px;
    height: 120px;
    object-fit: cover;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    flex-shrink: 0;
}

/* --- Typography Details --- */
.menu-details {
    flex-grow: 1;
}

.menu-details h3 {
    margin: 0 0 5px 0;
    font-size: 1.25rem;
    color: #2c3e50;
}

.menu-details p {
    margin: 0 0 10px 0;
    color: #666666;
    font-size: 0.95rem;
}

/* --- Sleek, Modern Price Styling --- */
.price-options {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    gap: 15px;
}

.price-options li {
    background: #f1f5f3;
    padding: 4px 10px;
    border-radius: 6px;
    font-size: 0.9rem;
}

.price-label {
    color: #555;
    font-weight: 500;
}

.price-value {
    color: #1b4d3e;
    font-weight: bold;
    margin-left: 5px;
}
/* --- Pure CSS Menu Tabs Functionality --- */

/* Hide the raw radio input circles */
.tab-input {
    display: none;
}

/* Style the tab buttons/labels container */
.tab-labels {
    display: flex;
    justify-content: center;
    gap: 10px;
    margin-bottom: 35px;
    flex-wrap: wrap;
    border-bottom: 2px solid #eaeaea;
    padding-bottom: 15px;
}

/* Style individual tab buttons */
.tab-labels label {
    background-color: #f1f5f3;
    color: #2c3e50;
    padding: 10px 20px;
    border-radius: 25px;
    cursor: pointer;
    font-weight: 600;
    transition: all 0.3s ease;
    font-size: 0.95rem;
}

.tab-labels label:hover {
    background-color: #d8e5e0;
    color: #1b4d3e;
}

/* Hide all menu sections by default */
.menu-section {
    display: none;
}

/* Connect the radio buttons to show the correct section when clicked */
#food-tab1:checked ~ .tab-labels label[for="food-tab1"],
#food-tab2:checked ~ .tab-labels label[for="food-tab2"],
#food-tab3:checked ~ .tab-labels label[for="food-tab3"],
#food-tab4:checked ~ .tab-labels label[for="food-tab4"] {
    background-color: #1b4d3e;
    color: #ffffff;
}

#food-tab1:checked ~ #appetizers,
#food-tab2:checked ~ #soup,
#food-tab3:checked ~ #main-courses,
#food-tab4:checked ~ #sweet {
    display: block;
    animation: fadeIn 0.4s ease-in-out;
}

/* Smooth fade-in effect when switching tabs */
@keyframes fadeIn {
    from { opacity: 0; transform: translateY(5px); }
    to { opacity: 1; transform: translateY(0); }
}




/* --- TABS COMPONENT STYLES --- */

/* 1. Hide the actual radio buttons */
.menu-container {
    max-width: 800px;
    margin: 40px auto;
    padding: 0 20px;
}

.tab-input {
    display: none;
}

/* 2. Style the tab labels to look like buttons */
.tab-labels {
    display: flex;
    justify-content: center;
    gap: 15px;
    margin-bottom: 30px;
}

.tab-labels label {
    background-color: #f0f0f0;
    color: #333;
    padding: 12px 24px;
    font-weight: bold;
    border-radius: 4px;
    cursor: pointer;
    transition: background-color 0.3s ease, color 0.3s ease;
}

.tab-labels label:hover {
    background-color: #ddd;
}

/* 3. Hide all content sections by default */
.menu-container .content {
    display: none;
}

/* 4. Show the correct content and highlight active tab based on checked radio */
#tab1:checked ~ .tab-labels label[for="tab1"],
#tab2:checked ~ .tab-labels label[for="tab2"] {
    background-color: #333; /* Darker accent for active tab */
    color: #fff;
}

#tab1:checked ~ #drinks-content {
    display: block;
}

#tab2:checked ~ #coffee-content {
    display: block;
}

/* 5. Menu Item Styling for Clean Layout */
.content h2, .content h3 {
    border-bottom: 2px solid #eaeaea;
    padding-bottom: 8px;
    margin-top: 30px;
    margin-bottom: 15px;
    color: #2c2c2c;
}

.item {
    display: flex;
    justify-content: space-between;
    padding: 10px 0;
    border-bottom: 1px dashed #ddd;
}

.item p {
    margin: 0;
}

.item p:last-child {
    font-weight: bold;
    color: #b17b38; /* Warm accent matching restaurant vibe */
}



/* ==========================================
   Cedar House - About Page & Global Clean-up
   ========================================== */

/* Global Styles - Modernized Clean Font */
body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #fcfbfa;
    color: #333333;
    line-height: 1.6;
}

header {
    text-align: center;
    padding: 25px 20px;
    background-color: #ffffff;
    border-bottom: 1px solid #eaeaea;
}

header img {
    display: block;
    margin: 0 auto 10px auto;
}

header h1 {
    margin: 0;
    font-size: 2.2rem;
    color: #1a1a1a;
    letter-spacing: 0.5px;
}

/* Navigation Styles */
.nav-container {
    background-color: #ffffff;
    border-bottom: 1px solid #eaeaea;
    padding: 12px 0;
}

.nav-horizontal {
    list-style: none;
    display: flex;
    justify-content: center;
    gap: 30px;
    margin: 0;
    padding: 0;
}

.nav-horizontal li a {
    text-decoration: none;
    color: #555555;
    font-size: 0.95rem;
    font-weight: 500;
    transition: color 0.2s ease;
}

.nav-horizontal li a:hover {
    color: #b8a26e;
}

/* Active navigation link styling */
.nav-horizontal a.active {
    font-weight: bold;
    color: #b8a26e;
}



/* Styling for your Story Section */
main section {
    max-width: 800px; /* Keeps lines from getting too long, which improves readability */
    margin: 0 auto;   /* Centers the section */
    padding: 40px 20px;
}

main section p {
    font-size: 1.1rem;      /* Slightly larger for readability */
    line-height: 1.8;       /* Increases space between lines for a cleaner look */
    margin-bottom: 25px;    /* Adds space between paragraphs */
    color: #333;            /* Dark grey instead of harsh black */
    text-align: justify;    /* Aligns text evenly for a clean, blocky look */
    font-family: 'Georgia', serif; /* A classic, professional serif font */
}

/* Styling for your caption */
figcaption {
    font-size: 0.9rem;
    color: #777;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    margin-top: 10px;
    margin-bottom: 30px;
}


body {
    margin: 0;
    padding: 0;
    font-family: sans-serif;
    background-color: #f4f4f4;
}

/* Centers everything inside the div */
.form-container {
    max-width: 600px;
    margin: 40px auto; /* Centers the block on the page */
    padding: 30px;
    background-color: #ffffff;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

h1 {
    font-family: 'Playfair Display', serif;
    text-align: center;
    color: #333;
}

.gallery-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin: 20px 0;
}

.gallery-container img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    border-radius: 8px;
}

fieldset {
    border: none;
    margin-bottom: 25px;
    padding: 0;
}

legend {
    font-size: 1.5rem;
    color: #b8a26e;
    border-bottom: 1px solid #b8a26e;
    width: 100%;
    margin-bottom: 15px;
}

input, select, textarea {
    width: 100%;
    padding: 12px;
    margin-bottom: 15px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
}

.btn-primary {
    width: 100%;
    background-color: #b8a26e;
    color: white;
    padding: 15px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    text-transform: uppercase;
}

@media (max-width: 768px) {
    .gallery-container {
        grid-template-columns: 1fr;
    }
}



.order-online {
    padding: 40px;
    text-align: center;
}

.order-options {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}

.order-card {
    width: 220px;
    padding: 20px;
    border-radius: 12px;
    background-color: white;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
}

.order-card a {
    display: inline-block;
    margin-top: 10px;
    padding: 10px 15px;
    text-decoration: none;
    border-radius: 8px;
    background-color: #333;
    color: white;
}






.jobs-page {
    width: 80%;
    margin: 40px auto;
}

.jobs-page form input,
.jobs-page form select,
.jobs-page form textarea {
    width: 100%;
    padding: 10px;
    margin-top: 5px;
}

.jobs-page button {
    padding: 12px 24px;
    cursor: pointer;
}


/* Style inputs with type="text", type="email", type="tel", date, select elements and textareas */
input[type=text], input[type=email], input[type=tel], input[type=date], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
  margin-top: 6px;
  margin-bottom: 16px;
  resize: vertical;
}

/* Style the submit and reset buttons */
input[type=submit], input[type=reset] {
  background-color: #04AA6D;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  margin-right: 10px;
}

input[type=reset] {
  background-color: #ccc;
  color: #333;
}

input[type=submit]:hover {
  background-color: #45a049;
}

input[type=reset]:hover {
  background-color: #b3b3b3;
}

/* Add a background color and some padding around the form */
.container {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}

fieldset {
  border: 1px solid #0000FF;
  margin-bottom: 20px;
  padding: 15px;
  border-radius: 4px;
}

legend {
  color: #0000FF;
  font-weight: bold;
}