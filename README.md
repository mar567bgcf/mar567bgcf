<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Website</title>
    <link rel="stylesheet" href="styles.css">
<body>
    <h1>Hello, World!</h1>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    text-align: center;
}

h1 {
    color: #333;
}
alert("Welcome to Your Website!");
const express = require('express');
const app = express();
const port = process.env.PORT || 3000;

app.use(express.static('public'));

app.get('/', (req, res) => {
    res.sendFile(__dirname + '/public/index.html');
});

app.listen(port, () => {
    console.log(`Server is running at http://localhost:${port}`);
});
project-root
├── public
│   ├── index.html
│   ├── styles.css
│   └── script.js
├── server.js
└── README.md
