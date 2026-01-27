# resume-page
resume/
│── index.html
│── style.css
│── script.js
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Hemanth Kumar J - Resume</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Folder Section -->
    <div class="folder-container">
        <div class="folder" onclick="openResume()">
            📁 Hemanth_Kumar_J
        </div>
    </div>

    <!-- Full Screen Resume -->
    <div id="resumeOverlay">
        <div class="resume-box">
            <h1>HEMANTH KUMAR J</h1>

            <div class="info-box">First Name: Hemanth</div>
            <div class="info-box">Last Name: Kumar J</div>
            <div class="info-box">Date of Birth: DD / MM / YYYY</div>
            <div class="info-box">Contact Number: 8147414701</div>
            <div class="info-box">Email ID: hemanthkumarj080@gmail.com</div>
            <div class="info-box">Location: Bengaluru, Karnataka</div>

            <h2>Skills</h2>
            <div class="info-box">Project Management</div>
            <div class="info-box">Software Development</div>
            <div class="info-box">UI / UX Design</div>
            <div class="info-box">Business Analysis</div>
            <div class="info-box">Staff & User Training</div>

            <div class="footer-border">
                IMTDA INFO TECH PRIVATE LIMITED
            </div>

            <button class="close-btn" onclick="closeResume()">Close</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    background: #f4f6f8;
}

/* Folder Style */
.folder-container {
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

.folder {
    padding: 20px 40px;
    border: 2px solid #333;
    cursor: pointer;
    font-size: 22px;
    background: white;
    transition: 0.3s;
}

.folder:hover {
    background: #333;
    color: white;
}

/* Overlay Resume */
#resumeOverlay {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.85);
    overflow-y: auto;
}

/* Resume Box */
.resume-box {
    background: white;
    max-width: 800px;
    margin: 40px auto;
    padding: 40px;
    border-radius: 10px;
    box-shadow: 0 0 25px rgba(0,0,0,0.3);
}

/* Headings */
.resume-box h1 {
    text-align: center;
    border-bottom: 2px solid #444;
    padding-bottom: 10px;
}

.resume-box h2 {
    margin-top: 30px;
    border-left: 5px solid #444;
    padding-left: 10px;
}

/* Info Boxes */
.info-box {
    border: 1px solid #ccc;
    padding: 12px;
    margin: 10px 0;
    border-radius: 5px;
    background: #fafafa;
}

/* Footer Company Name */
.footer-border {
    margin-top: 40px;
    text-align: center;
    padding: 15px;
    border-top: 2px solid #000;
    border-bottom: 2px solid #000;
    font-weight: bold;
    letter-spacing: 1px;
}

/* Close Button */
.close-btn {
    display: block;
    margin: 30px auto 0;
    padding: 10px 25px;
    border: none;
    background: #333;
    color: white;
    cursor: pointer;
    border-radius: 5px;
}

.close-btn:hover {
    background: #000;
}
function openResume() {
    document.getElementById("resumeOverlay").style.display = "block";
}

function closeResume() {
    document.getElementById("resumeOverlay").style.display = "none";
}
