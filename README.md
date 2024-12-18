# Ex.08 Design of Interactive Image Gallery
## Date:15/12/2024

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
```
index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image gallery</title>
    <link rel="stylesheet" href="style.css">
    <script src="index.js" defer></script>
</head>
<body>
    <h1 align="center">Interactive Image Gallery</h1>
 
<div class="container">
    <div class="gallery">
        <img src="Untitled.webp" onclick="openFullImg(this.src)">
        <img src="ak11.webp" onclick="openFullImg(this.src)">
        <img src="kojima.jpg" onclick="openFullImg(this.src)">
        <img src="bezos.webp" onclick="openFullImg(this.src)">
        <img src="bill.webp" onclick="openFullImg(this.src)">
        <img src="dhanush1.webp" onclick="openFullImg(this.src)">
        
    </div>

</div>
<div class="fullimg" id="fullImgBox">
    <img src="Untitled.webp" id="fullImg">
    <span onclick="closeFullImg()">X</span>
</div>  
<footer>
    <p align="center">&copy; Designed and developed by K Barathraj</p>
</footer>
</body>

</html>

index.js

var fullImgBox = document.getElementById("fullImgBox");
var fullImg = document.getElementById("fullImg");
function openFullImg(pic){
    fullImgBox.style.display="flex";
    fullImg.src = pic;
}
function closeFullImg(){
    fullImgBox.style.display="none";
}

style.css


*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family:'poppins',sans-serif;
    background-image: url(back11.jpg);
}
.container{
    flex: 1; 
    display: flex;
    flex-direction: column;
    align-items: center; 
    justify-content: center; 
}
h1 {
    width: 100%;
    text-align: center;
    margin-bottom: 20px;
    color: rgb(0, 255, 64);
    font-family: cursive;
}
.gallery{
    display: grid;
    grid-template-columns: repeat(3,auto);
    grid-gap: 30px;
}
.gallery img{
    width: 100%;
    cursor: pointer;
}
.fullimg{
    width: 100%;
    height: 100vh;
    background: rgba(0,0,0,0.9);
    position: fixed;
    top: 0;
    left: 0;
    display: none;align-items: center;
    justify-content: center;
}
.fullimg img{
    width:90%;
    max-width: 500px;
}
.fullimg span{
    position: absolute;
    top: 5%;
    right:5%;
    font-size: 30px;
    color:white;
    cursor: pointer;
}
footer {
    text-align: center;
    padding: 10px;
    background-color: #222; 
    color: white;
}


```
## OUTPUT:
![alt text](image-1.png)
![alt text](image.png)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
