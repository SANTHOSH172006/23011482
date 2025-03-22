## INTERACTIVE IMAGE GALLERY


## Name : SANTHOSH D
## Reg. No: 212223220099
## Date : 22-03-2025

## AIM:
Design and implement an interactive image gallery using JavaScript, HTML, and CSS.

## ALGORITHM:

### STEP 1
Display multiple images in a horizontal scrollable layout.

### STEP 2
Each image must have a caption that appears when hovered over.

### STEP 3
Include Next and Previous buttons to navigate through the images.

### STEP 4
Use JavaScript to enhance interactivity (e.g., smooth sliding animations, hover effects).

### STEP 5
Style the gallery using CSS for a visually appealing and responsive design.

### STEP 6
Include a footer at the bottom of the page with the text “Learner’s Name and Register Number”.

### STEP 7
Your solution should include well-structured HTML, CSS, and JavaScript code, ensuring smooth user experience and navigation.

## PROGRAM:
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>TOP TAMIL FILM ACTORS</h1><br><br>
    <div class="gallery-container">
        <div class="gallery" id="gallery">
            <div class="image-container">
                <img src="download.jpeg" alt="Image 1">
                <div class="caption">Caption 1 - vijay</div>
            </div>
            <div class="image-container">
                <img src="Kamal_haasan.jpg" alt="Image 2">
                <div class="caption">Caption 2 - kamal</div>
            </div>
            <div class="image-container">
                <img src="surya.jpeg" alt="Image 3">
                <div class="caption">Caption 3 - suriya</div>
            </div>
            <div class="image-container">
                <img src="rajin.avif" alt="Image 4">
                <div class="caption">Caption 4 - Rajini</div>
            </div>
            <div class="image-container">
                <img src="SivakarthikeyanActor.jpg" alt="Image 5">
                <div class="caption">Caption 5 - sk</div>
            </div>
           
        </div>
    </div><br><br><br>
    <div class="controls">
        <button onclick="scrollGallery(-500)">Previous</button>
        <button onclick="scrollGallery(500)">Next</button>
    </div><br><br><br><br><br><br>
    <div class="footer">
        <p>&copy; 2025 Santhosh d 212223220099. All rights reserved.</p>
    </div>
    <script src="script.js"></script>
</body>
</html>
```
style.css
```
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    text-align: center;
    background-color: cyan;
}
.gallery-container {
    position: relative;
    width: 80%;
    margin: auto;
    overflow: hidden;
}
.gallery {
    display: flex;
    overflow-x: scroll;
    scroll-behavior: smooth;
    padding: 10px;
    white-space: nowrap;
}
.gallery img {
    width: 250px;
    height: 250px;
    margin: 10px;
    object-fit: cover;
    border-radius: 10px;
    transition: transform 0.3s ease-in-out;
    position: relative;
}
.gallery img:hover {
    transform: scale(1.1);
}
.caption {
    position: absolute;
    background: rgba(0, 0, 0, 0.7);
    color: white;
    width: 300px;
    text-align: center;
    padding: 5px;
    bottom: 10px;
    opacity: 0;
    transition: opacity 0.3s ease-in-out;
    border-radius: 10px;
}
.image-container {
    position: relative;
    display: inline-block;
}
.image-container:hover .caption {
    opacity: 1;
}
.controls {
    margin-top: 20px;
}
.controls button {
    padding: 10px 20px;
    margin: 5px;
    border: none;
    cursor: pointer;
    background-color: #007BFF;
    color: white;
    border-radius: 5px;
    font-size: 16px;
}
.controls button:hover {
    background-color: #0056b3;
}
.footer {
    margin-top: 20px;
    padding: 10px;
    background: #333;
    color: white;
}
```
script.js
```
function scrollGallery(direction) {
    document.getElementById('gallery').scrollBy({
        left: direction,
        behavior: 'smooth'
    });
}
```
## OUTPUT:
![web atten](https://github.com/user-attachments/assets/511cc38e-9a6d-430b-8c49-8042974fbaa6)


## RESULT:
The program for creating Interactive Image Gallery using HTML,CSS and Javascript is executed successfully.
