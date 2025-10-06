# Ex.08 Design of Interactive Image Gallery
## Date:06.10.2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Marvel Gallery</title>

  <!-- Google Font (for comic style) -->
  <link href="https://fonts.googleapis.com/css2?family=Bangers&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Bangers', cursive;
      background-image: url('background.jpg');
      background-size: cover;
      background-attachment: fixed;
      background-position: center;
      color: white;
      text-align: center;
    }

    h1 {
      font-size: 3rem;
      color: #ff1c1c;
      text-shadow: 2px 2px 8px black;
      margin-top: 40px;
      letter-spacing: 3px;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 25px;
      padding: 40px;
      max-width: 1200px;
      margin: auto;
    }

    .card {
      position: relative;
      overflow: hidden;
      border-radius: 15px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.6);
      transition: transform 0.4s ease, box-shadow 0.4s ease;
    }

    .card img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.5s ease;
    }

    .card:hover {
      transform: scale(1.05);
      box-shadow: 0 10px 25px rgba(255, 0, 0, 0.6);
    }

    .card:hover img {
      transform: scale(1.1);
    }

    .overlay {
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      height: 0;
      background: rgba(0, 0, 0, 0.7);
      color: white;
      overflow: hidden;
      transition: height 0.4s ease;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
      letter-spacing: 2px;
    }

    .card:hover .overlay {
      height: 40%;
    }
  </style>
</head>
<body>

  <h1>Marvel Legends Gallery</h1>

  <div class="gallery">
    <div class="card">
      <img src="ironman.jpg" alt="Iron Man">
      <div class="overlay">Iron Man</div>
    </div>
    <div class="card">
      <img src="captain-america-marvel-comics_1200x.webp" alt="Captain America">
      <div class="overlay">Captain America</div>
    </div>
    <div class="card">
      <img src="68961_627x.webp" alt="Thor">
      <div class="overlay">Thor</div>
    </div>
    <div class="card">
      <img src="images (1).jpg" alt="Hulk">
      <div class="overlay">Hulk</div>
    </div>
    <div class="card">
      <img src="spiderman-marvel-rivals-g3.jpg" alt="Spider-Man">
      <div class="overlay">Spider-Man</div>
    </div>
    <div class="card">
      <img src="black-widow.webp" alt="Black Widow">
      <div class="overlay">Black Widow</div>
    </div>
    <div class="card">
      <img src="Dr_strange_by_joeyvazquez-dbdnuf1.webp" alt="Doctor Strange">
      <div class="overlay">Doctor Strange</div>
    </div>
    <div class="card">
      <img src="Black_Panther_OS_Vol_1_2.png" alt="Black Panther">
      <div class="overlay">Black Panther</div>
    </div>
  </div>

</body>
</html>

```
## OUTPUT:
<img width="1893" height="922" alt="Screenshot 2025-10-06 145219" src="https://github.com/user-attachments/assets/a258ff82-0841-4ace-807e-4da3e6849e6e" />

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
