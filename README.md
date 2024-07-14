<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IO Game Maker</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>IO Game Maker</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#create">Create Game</a></li>
                <li><a href="#discover">Discover</a></li>
                <li><a href="#login">Login</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h2>Welcome to IO Game Maker</h2>
        <p>Create and discover amazing .io games!</p>
    </section>

    <section id="create">
        <h2>Create Your Game</h2>
        <button onclick="showGameEditor()">Start Creating</button>
        <div id="game-editor" style="display:none;">
            <div class="toolbar">
                <button onclick="addSprite()">Add Sprite</button>
                <button onclick="addBackground()">Add Background</button>
                <button onclick="setProperties()">Set Properties</button>
                <button onclick="saveGame()">Save Game</button>
                <button onclick="publishGame()">Publish Game</button>
            </div>
            <div id="game-canvas">
                <!-- Game creation canvas will be here -->
            </div>
        </div>
    </section>

    <section id="discover">
        <h2>Discover Games</h2>
        <input type="text" id="search-bar" placeholder="Search for games...">
        <button onclick="searchGames()">Search</button>
        <div id="game-list">
            <!-- Games will be listed here -->
        </div>
    </section>

    <section id="login">
        <h2>Login or Sign Up</h2>
        <form id="login-form">
            <input type="email" id="email" placeholder="Email">
            <input type="password" id="password" placeholder="Password">
            <button type="button" onclick="login()">Login</button>
            <button type="button" onclick="signUp()">Sign Up</button>
        </form>
    </section>

    <script src="script.js"></script>
</body>
</html>
