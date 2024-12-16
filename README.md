<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Anniversary</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f8ff;
            font-family: Arial, sans-serif;
        }
        #message {
            display: none;
            font-size: 2em;
            color: #ff69b4;
        }
        a {
            font-size: 1.5em;
            color: #1e90ff;
            text-decoration: none;
        }
    </style>
</head>
<body>

<a href="#" id="showMessage">Click here for a surprise!</a>
<div id="message">Happy Anniversary, Dear!...Love you!</div>

<script>
    document.getElementById('showMessage').addEventListener('click', function(event) {
        event.preventDefault(); // Prevent the default link behavior
        document.getElementById('message').style.display = 'block'; // Show the message
        this.style.display = 'none'; // Hide the link
    });
</script>

</body>
</html>
