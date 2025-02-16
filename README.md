<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>birthday💗 Day Surprise</title>
    <style>
        body {
            text-align: center;
            background: url('https://i.imgur.com/3mYsMQw.png') no-repeat center center fixed; /* Hello Kitty background */
            background-size: cover;
            font-family: 'Arial', sans-serif;
            color: white;
        }
        #content {
            display: none;
            margin-top: 20%;
        }
        .message {
            font-size: 30px;
            font-weight: bold;
            background: rgba(0, 0, 0, 0.6);
            padding: 20px;
            border-radius: 15px;
            display: inline-block;
        }
        #login {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        input, button {
            padding: 10px;
            font-size: 18px;
            margin: 10px;
            border: none;
            border-radius: 5px;
        }
        button {
            background: pink;
            cursor: pointer;
        }
    </style>
</head>
<body>

<div id="login">
    <h2>What's one pet Nancy would love to have?</h2>
    <input type="text" id="answer" placeholder="Enter your answer...">
    <button onclick="checkAnswer()">Submit</button>
</div>

<div id="content">
    <audio autoplay loop>
        <source src="your-audio-file.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>
    <div class="message">
        💝 Happy birthday, 💖 <br>
        "I like me better when I'm with you!"
    </div>
</div>

<script>
    function checkAnswer() {
        let userAnswer = document.getElementById("answer").value.toLowerCase();
        if (userAnswer === "dog" || userAnswer === "puppy") {
            document.getElementById("login").style.display = "none";
            document.getElementById("content").style.display = "block";
        } else {
            alert("Oops! Try again.");
        }
    }
</script>

</body>
</html>
