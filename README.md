![Screenshot 2025-03-22 135124](https://github.com/user-attachments/assets/00bc8f8d-e326-45ad-b358-971b630135eb)# github.io-Gallery# Activity 01 
## Date: 22.03.2025

## AIM
Design and implement an interactive image gallery using JavaScript, HTML, and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Create a JS file (script.js)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the Gallery, image, and footer.

### STEP 7
Use CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
</head>
<body>
    <header>
        <h1>Interactive Image Gallery</h1>
    </header>
    <div class="gallery-container">
        <button id="prevBtn" class="nav-btn">&#10094;</button>
        <div class="gallery-wrapper">
            <div class="gallery" id="gallery">
                <div class="image-container" style="background-image: url('images/csk.png');">
                    <span class="caption">Consistent performance, strong leadership, and experienced players.                    </span>
                </div>
                <div class="image-container" style="background-image: url('images/kkr.png');">
                    <span class="caption">Aggressive gameplay, star power, and passionate fan base.</span>
                </div>
                <div class="image-container" style="background-image: url('images/rcb.png');">
                    <span class="caption">Star players like Virat Kohli & AB de Villiers, strong batting lineup.</span>
                </div>
                <div class="image-container" style="background-image: url('images/srh.png');">
                    <span class="caption">Exceptional bowling attacks and solid team balance.</span>
                </div>
            </div>
        </div>
        <button id="nextBtn" class="nav-btn">&#10095;</button>
    </div>
    <footer>
        <p> Shyam  -  212223040200</p>
    </footer>
</body>
</html>
```

style.css
```
body {
    font-family: Arial, sans-serif;
    background-color: #f5f5f5;
    margin: 0;
    padding: 0;
    text-align: center;
}

header {
    background-color: #333;
    color: white;
    padding: 15px 0;
    font-size: 24px;
}

.gallery-container {
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    margin: 20px auto;
    width: 80%;
    overflow: hidden;
}

.gallery-wrapper {
    overflow-x: hidden;
    width: 100%;
}

.gallery {
    display: flex;
    transition: transform 0.5s ease-in-out;
}

.image-container {
    min-width: 300px;
    height: 200px;
    background-size: cover;
    background-position: center;
    position: relative;
    margin: 10px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    cursor: pointer;
    transition: transform 0.3s ease;
}

.image-container:hover {
    transform: scale(1.05);
}

.caption {
    position: absolute;
    bottom: 0;
    background: rgba(0, 0, 0, 0.6);
    color: white;
    width: 100%;
    text-align: center;
    padding: 10px;
    opacity: 0;
    transition: opacity 0.3s ease;
}

.image-container:hover .caption {
    opacity: 1;
}

.nav-btn {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(0, 0, 0, 0.7);
    color: white;
    border: none;
    cursor: pointer;
    padding: 10px;
    font-size: 24px;
    transition: background 0.3s ease;
}

.nav-btn:hover {
    background-color: rgba(0, 0, 0, 0.9);
}

#prevBtn {
    left: 10px;
}

#nextBtn {
    right: 10px;
}

footer {
    background-color: #333;
    color: white;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
}

```

script.js
```
document.addEventListener("DOMContentLoaded", function () {
    const gallery = document.getElementById("gallery");
    const prevBtn = document.getElementById("prevBtn");
    const nextBtn = document.getElementById("nextBtn");

    let scrollAmount = 0;
    const scrollStep = 320;

    nextBtn.addEventListener("click", () => {
        gallery.scrollTo({
            left: (scrollAmount += scrollStep),
            behavior: "smooth",
        });
    });

    prevBtn.addEventListener("click", () => {
        gallery.scrollTo({
            left: (scrollAmount -= scrollStep),
            behavior: "smooth",
        });
    });
});

```

## OUTPUT

![Screenshot 2025-03-22 135124](https://github.com/user-attachments/assets/7b1542f9-a1ad-41a0-a7e3-c961db4e2f71)

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
