# laxmi
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fun Facts Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }
        .container {
            text-align: center;
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .fact {
            font-size: 1.5em;
            margin: 20px 0;
        }
        .btn {
            background: #007BFF;
            color: #fff;
            border: none;
            padding: 10px 20px;
            font-size: 1em;
            cursor: pointer;
            border-radius: 5px;
        }
        .btn:hover {
            background: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="fact" id="fact">Click the button to see a fun fact!</div>
        <button class="btn" onclick="generateFact()">Generate Fun Fact</button>
    </div>
    <script>
        const facts = [
            "Honey never spoils.",
            "A group of flamingos is called a 'flamboyance'.",
            "Bananas are berries, but strawberries aren't.",
            "Octopuses have three hearts.",
            "There are more stars in the universe than grains of sand on Earth."
        ];

        function generateFact() {
            const randomIndex = Math.floor(Math.random() * facts.length);
            document.getElementById('fact').innerText = facts[randomIndex];
        }
    </script>
</body>
</html>
