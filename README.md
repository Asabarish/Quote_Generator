# Quote_Generator
## Date:14.3.2026
## Objective:
To create a simple thirukkural generator using HTML, CSS, and JavaScript that displays a new random thirukkural each time a button is clicked — similar to daily quote sections on blogs or productivity apps.

## Tasks:

### 1. Create the HTML Structure:
<ul>
  <li>Add a heading Thirukkural Generator</li>
  <li>Use a div or p to display the Thirukkural (Tamil couplet).</li>
  <li>Use another p or span to display the meaning or explanation.</li>
  <li>Add a button labeled “Get Thirukkural”.</li>
  <li>Add a label showing the Kural number.</li>
</ul>

### 2. Style the Layout Using CSS:

<ul>
  <li>Center everything on the page using Flexbox.</li>
  <li>Style the quote box with:
  <ul type="square">
    <li>Padding</li>
    <li>Background color</li>
    <li>Rounded borders</li>
    <li>Soft shadow</li>
    <li>Add hover effects for the button.</li>
  </ul>
  </li>
</ul>

### 3. Add JavaScript Functionality:
<ul>
  <li>Store an array of Thirukkural objects containing:
  <ul type="square">
    <li>Kural number</li>
    <li>Kural Meaning</li>
  </ul>
  </li>
  <li>When the button is clicked:
  <ul type="square">
    <li>Generate a random index using Math.random().</li>
    <li>Retrieve the corresponding Thirukkural object.</li>
    <li>Display the Kural number and meaning in the HTML.</li>
    <li>Update content dynamically using innerText.</li>
  </ul>
  </li>
</ul>

## Code:
```
index.html

<!DOCTYPE html>
<html>
<head>
<title>Thirukkural Generator</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<h1>Thirukkural Generator</h1>

<div class="box">
<p id="kural">Click the button to see a Thirukkural</p>

<button onclick="newKural()">Generate Kural</button>
</div>

<script src="script.js"></script>

</body>
</html>


style.css


body{
text-align:center;
font-family:Arial;
background:#f5f5f5;
}

h1{
color:#2c3e50;
}

.box{
background:white;
width:400px;
margin:auto;
padding:20px;
border-radius:10px;
box-shadow:0px 0px 10px gray;
}

button{
padding:10px 20px;
background:#27ae60;
color:white;
border:none;
border-radius:5px;
cursor:pointer;
}

button:hover{
background:#2ecc71;
}



script.js

function newKural(){

var kurals = [

"அகர முதல எழுத்தெல்லாம் ஆதி\nபகவன் முதற்றே உலகு",

"கற்றதனால் ஆய பயனென்கொல் வாலறிவன்\nநற்றாள் தொழாஅர் எனின்",

"அன்பிற்கும் உண்டோ அடைக்குந்தாழ் ஆர்வலர்\nபுன்கணீர் பூசல் தரும்",

"தீயினால் சுட்ட புண் உள்ளாறும் ஆறாதே\nநாவினால் சுட்ட வடு",

"ஒழுக்கம் விழுப்பம் தரலான் ஒழுக்கம்\nஉயிரினும் ஓம்பப் படும்"

];

var random = Math.floor(Math.random()*kurals.length);

document.getElementById("kural").innerText = kurals[random];

}

```
## Output:
![alt text](<Screenshot 2026-03-14 153202-1.png>) ![alt text](<Screenshot 2026-03-14 153211-1.png>) ![alt text](<Screenshot 2026-03-14 153221-1.png>) ![alt text](<Screenshot 2026-03-14 153141-1.png>) ![alt text](<Screenshot 2026-03-14 153151-1.png>)

## Result:
A simple quote generator using HTML, CSS, and JavaScript that displays a new random motivational quote each time a button is clicked — similar to daily quote sections on blogs or productivity apps is created successfully.
