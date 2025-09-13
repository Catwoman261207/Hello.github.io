<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I'm Sorry</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1 class="title">I'm Sorry...</h1>
        <button class="open-letter" onclick="openLetter()">Open Letter</button>
        <div class="game-container">
            <button class="play-game" onclick="startGame()">Play a Silly Game</button>
        </div>
    </div>

    <!-- Popup Open Letter -->
    <div class="letter-popup" id="letterPopup">
        <div class="letter-content">
            <h2>Open Letter</h2>
            <p id="letterText">Dear [Name],</p>
            <p>I'm really sorry for what happened. I know I messed up, and I promise I'll do better. I hope you can find it in your heart to forgive me. I’ll make it up to you, I swear! ❤️</p>
            <button class="close-popup" onclick="closeLetter()">Close</button>
        </div>
    </div>

    <!-- Game Popup -->
    <div class="game-popup" id="gamePopup">
        <div class="game-content">
            <h2>Why Should You Forgive Me?</h2>
            <p>Pick an option, and let's see why I deserve another chance!</p>
            <button class="answer" onclick="answer('Because I’ll buy you your favorite snack!')">I'll buy you your favorite snack!</button>
            <button class="answer" onclick="answer('I promise to never forget your birthday again!')">I promise to never forget your birthday again!</button>
            <button class="answer" onclick="answer('I’ll be your personal chef for a week!')">I’ll be your personal chef for a week!</button>
            <button class="close-game" onclick="closeGame()">Close Game</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
/* Basic Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background: #f7d2f7;
    color: #333;
    text-align: center;
}

.container {
    padding: 20px;
}

.title {
    font-size: 3rem;
    color: #ff69b4;
    margin-bottom: 20px;
}

.open-letter, .play-game {
    font-size: 1.2rem;
    padding: 10px 20px;
    border: none;
    background-color: #ff69b4;
    color: white;
    cursor: pointer;
    border-radius: 10px;
    transition: background-color 0.3s;
}

.open-letter:hover, .play-game:hover {
    background-color: #ff1493;
}

.letter-popup, .game-popup {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.6);
    justify-content: center;
    align-items: center;
}

.letter-content, .game-content {
    background: white;
    padding: 30px;
    border-radius: 10px;
    width: 60%;
    max-width: 500px;
    text-align: center;
}

.letter-content h2, .game-content h2 {
    font-size: 2rem;
    color: #ff69b4;
}

button {
    font-size: 1rem;
    padding: 10px 20px;
    background-color: #ff69b4;
    color: white;
    border: none;
    cursor: pointer;
    border-radius: 10px;
    margin-top: 10px;
    transition: background-color 0.3s;
}

button:hover {
    background-color: #ff1493;
}

.game-popup .answer {
    margin-bottom: 10px;
    width: 100%;
}

button.close-popup, button.close-game {
    background-color: #ff1493;
}

button.close-popup:hover, button.close-game:hover {
    background-color: #ff69b4;
}

.heart {
    position: absolute;
    animation: float 5s infinite;
}

@keyframes float {
    0% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-20px);
    }
    100% {
        transform: translateY(0);
    }
}
// Open and Close Letter
function openLetter() {
    document.getElementById('letterPopup').style.display = 'flex';
}

function closeLetter() {
    document.getElementById('letterPopup').style.display = 'none';
}

// Start the game
function startGame() {
    document.getElementById('gamePopup').style.display = 'flex';
}

// Close the game
function closeGame() {
    document.getElementById('gamePopup').style.display = 'none';
}

// Answer Function
function answer(reason) {
    alert("Thank you for forgiving me! Here's why: " + reason);
    closeGame();
}
