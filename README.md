<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mathematics Study Guide</title>
    <style>
        body, html { margin: 0; padding: 0; width: 100%; height: 100%; font-family: sans-serif; background: #fff; }
        .disguise { padding: 40px; color: #333; max-width: 800px; margin: 0 auto; line-height: 1.6; }
        h1 { color: #1a73e8; }
        iframe { width: 100%; height: 100%; border: none; display: none; position: fixed; top: 0; left: 0; z-index: 99999; }
    </style>
</head>
<body>

    <!-- THE FAKE DISGUISE PAGE -->
    <div id="schoolWork" class="disguise">
        <h1>Chapter 4: Linear Equations & Graphs</h1>
        <p>A linear equation is an algebraic equation in which each term is either a constant or the product of a constant and a single variable. Linear equations can have one or more variables.</p>
        <hr>
        <h3>Practice Problems</h3>
        <p>1. Solve for x: 3x + 5 = 14</p>
        <p>2. Find the slope of the line passing through (2, 3) and (4, 7).</p>
        <p><i>Review notes thoroughly before the Friday exam.</i></p>
    </div>

    <!-- THE HIDDEN GAME -->
    <iframe id="gameFrame" src="https://shellgame.me"></iframe>

    <script>
        // TRICK: Press the "S" and "S" keys sequentially (or hold them) to unlock the game!
        let keysPressed = {};
        
        window.addEventListener('keydown', (event) => {
            keysPressed[event.key.toLowerCase()] = true;
            
            // If you press 's' and 'g' together (Secret Game)
            if (keysPressed['s'] && keysPressed['g']) {
                document.getElementById('schoolWork').style.display = 'none';
                document.getElementById('gameFrame').style.display = 'block';
            }
        });

        window.addEventListener('keyup', (event) => {
            delete keysPressed[event.key.toLowerCase()];
        });
    </script>
</body>
</html>
