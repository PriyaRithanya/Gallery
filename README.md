# Ex.08 Design of Interactive Image Gallery
# Date:8/10/25
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
gallery.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Interactive Photo Gallery</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <h1>Interactive Photo Gallery</h1>
  <div class="gallery">
    <div class="main-image">
      <img id="displayed-image" src="home1.jpg" alt="Main Display" />
    </div>
    <div class="houses">
      <img src="home1.jpg" onclick="changeImage(this)" alt="home1.jpg" />
      <img src="home2.jpg" onclick="changeImage(this)" alt="home2.jpg" />
      <img src="home3.jpeg" onclick="changeImage(this)" alt="home3.jpeg" />
      <img src="home4.jpg" onclick="changeImage(this)" alt="home4.jpg" />
      <img src="home5.jpg" onclick="changeImage(this)" alt="home5.jpg" />
    </div>
  </div>
  <script src="index.js"></script>
</body>
</html>

style.css

body {
  font-family: Arial, sans-serif;
  text-align: center;
  background-color: #162adc;
}

.gallery {
  max-width: 800px;
  margin: auto;
}

.main-image img {
  width: 100%;
  max-height: 500px;
  object-fit: cover;
  border: 2px solid #333;
}

.houses {
  margin-top: 20px;
  display: flex;
  justify-content: center;
  gap: 10px;
}

.houses img {
  width: 100px;
  height: 70px;
  object-fit: cover;
  cursor: pointer;
  border: 2px solid transparent;
  transition: border 0.3s;
}
.houses img:hover {
  border: 20px solid #090904;
}

index.js

function changeImage(element) {
  const mainImage = document.getElementById('displayed-image');
  mainImage.src = element.src;
  mainImage.alt = element.alt;
}

```
# OUTPUT:

![alt text](<Screenshot (41).png>)
![alt text](<Screenshot (42).png>)

# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
