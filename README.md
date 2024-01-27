# Tahlia-My-Love
Website dedicated to my girlfriend
<!DOCTYPE html>
<html>
<head>
    <title>Tahlia, My Love</title>
    <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>

    <header>
        <h1 id="header-title">Tahlia, My Love</h1>
    </header>

    <div class="sub-header">
        <h2>There is a light in your eyes and they never go out</h2>
    </div>

    <div id="youtube-playlist">
        <iframe src="https://www.youtube.com/embed/videoseries?list=PLYgM1VJb_kbUZHQYSUjm8v5DV0EVsmhES" frameborder="0" allowfullscreen></iframe>
    </div>

    <div id="poem-content">
        <p id="poem">"When we lock eyes and you start to head towards my direction the air feels different. My heart leaves my chest. It leaves because it knows where its true home is. It's always been you. Loving you is easy and I'm sorry if I ever it made it seem hard. I've lived a life before you and a life after you and both are lives I never want to live again. There's not enough time in my life to dedicate to you and show how much I love you. I plan on doing it anyway. You are my home. I need you like the tide needs the moon. Forever and always yours, Gabert"</p>
    </div>

    <script src="script.js"></script>
</body>
</html>

body {
    font-family: 'Times New Roman', serif;
    margin: 0;
    padding: 0;
    background-image: url('https://i.imgur.com/71YztNv.png');
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat;
}

header, .sub-header {
    text-align: center;
    background-color: rgba(255, 255, 255, 0.8);
    padding: 20px 0;
}

#header-title {
    font-family: 'Brush Script MT', cursive;
    color: #fffff;
    font-size: 48px;
}

.sub-header h2 {
    font-family: 'Times New Roman', serif; /* Same font as the poem */
    font-size: 32px; /* Adjust size as needed */
    color: #000; /* Color of the text */
    margin: 0;
}

#youtube-playlist {
    text-align: center;
    padding: 20px 0;
}

#youtube-playlist iframe {
    width: 560px;
    height: 315px;
    margin: 0 auto;
}

#poem-content {
    background-color: rgba(255, 255, 255, 0.8);
    margin: 20px;
    padding: 20px;
    text-align: center;
}

var slideIndex = 0;
showSlides();

function showSlides() {
    var i;
    var slides = document.getElementsByClassName("mySlides");
    for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";  
    }
    slideIndex++;
    if (slideIndex > slides.length) {slideIndex = 1}    
    slides[slideIndex-1].style.display = "block";  
    setTimeout(showSlides, 4000); // Change image every 4 seconds
