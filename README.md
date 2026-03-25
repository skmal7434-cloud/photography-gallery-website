<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Photography Gallery</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<nav>
    <h2>My Gallery</h2>
</nav>

<header>
    <h1>Photography Gallery</h1>
    <p>By Houssam Mohammad Hassan</p>
</header>

<section class="gallery">
    <img src="https://picsum.photos/300/200?1" onclick="openImage(this.src)">
    <img src="https://picsum.photos/300/200?2" onclick="openImage(this.src)">
    <img src="https://picsum.photos/300/200?3" onclick="openImage(this.src)">
    <img src="https://picsum.photos/300/200?4" onclick="openImage(this.src)">
    <img src="https://picsum.photos/300/200?5" onclick="openImage(this.src)">
    <img src="https://picsum.photos/300/200?6" onclick="openImage(this.src)">
</section>

<div id="lightbox" onclick="closeImage()">
    <img id="lightbox-img">
</div>

<footer>
    <p>© 2026 Photography Website</p>
</footer>

<script>
function openImage(src) {
    document.getElementById("lightbox").style.display = "flex";
    document.getElementById("lightbox-img").src = src;
}

function closeImage() {
    document.getElementById("lightbox").style.display = "none";
}
</script>

</body>
</html>
