# day-16-assign
# Auto Save Text Area
here i have created this project using html css java
## Step 1  Create a html file 

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>


    <div id="main">
        <div id="text">
            <h1>Auto Save Textarea</h1>
            <textarea placeholder="Start typing here.." name="" id="area" cols="30" rows="10"></textarea>
    </div>
    </div>

    <script src="script.js"></script>
</body>
</html>

## Step 2 creating a js file
const area = document.getElementById("area");

area.addEventListener("input", function() {
    const words = area.value.split(" ");

    localStorage.setItem("words", JSON.stringify(words));
});

## Step 3 here we will give styling using css and then deploy html file on browser
