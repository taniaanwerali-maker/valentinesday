<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine?</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            background-color: pink;
            font-family: Arial, sans-serif;
            text-align: center;
        }
        h1 {
            font-size: 2em;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 10px;
        }
        .yes-btn {
            background-color: red;
            color: white;
        }
        .no-btn {
            background-color: gray;
            color: white;
        }
        .locked-message {
            display: none;
            font-size: 2em;
            color: white;
        }
        .locked-image {
            display: none;
            width: 300px;
            border-radius: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1 id="question">Will you be my Valentine? ❤️</h1>
    <div class="buttons">
        <button class="yes-btn" onclick="lockLove()">Yes</button>
        <button class="no-btn" onclick="notAllowed()">No</button>
    </div>
    <h1 class="locked-message" id="lockedMessage">You're forever locked ❤️</h1>
    <img class="locked-image" id="lockedImage" src="/mnt/data/WhatsApp Image 2025-02-13 at 16.29.06_acff812d.jpg" alt="Locked Image">
    
    <script>
        function lockLove() {
            document.getElementById("question").style.display = "none";
            document.querySelector(".buttons").style.display = "none";
            document.getElementById("lockedMessage").style.display = "block";
            document.getElementById("lockedImage").style.display = "block";
        }
        
        function notAllowed() {
            alert("Not allowed!");
        }
    </script>
</body>
</html>
