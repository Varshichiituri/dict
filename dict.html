<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dictionary App</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4, #fad0c4, #ffdde1);
            margin: 0;
        }
        .container {
            background: white;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
            text-align: center;
            width: 90%;
            max-width: 400px;
            transition: transform 0.3s ease-in-out;
        }
        .container:hover {
            transform: scale(1.05);
        }
        input {
            width: 85%;
            padding: 12px;
            margin: 10px 0;
            border: none;
            border-radius: 8px;
            outline: none;
            font-size: 16px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        button {
            padding: 12px 20px;
            border: none;
            background: #ff6f61;
            color: white;
            font-size: 16px;
            border-radius: 8px;
            cursor: pointer;
            transition: background 0.3s;
        }
        button:hover {
            background: #e0524d;
        }
        #result {
            margin-top: 20px;
            font-size: 18px;
            font-weight: bold;
            color: #333;
        }
        h2 {
            color: #ff4757;
            font-size: 24px;
        }
        .audio-btn {
            margin-top: 10px;
            padding: 8px 15px;
            background: #28a745;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .audio-btn:hover {
            background: #218838;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Dictionary App</h2>
        <input type="text" id="word" placeholder="Enter a word...">
        <button onclick="searchWord()">Search</button>
        <div id="result"></div>
    </div>

    <script>
        async function searchWord() {
            let word = document.getElementById('word').value;
            let resultDiv = document.getElementById('result');
            resultDiv.innerHTML = "Loading...";
            try {
                let response = await fetch(`https://api.dictionaryapi.dev/api/v2/entries/en/${word}`);
                let data = await response.json();
                if (data.title) {
                    resultDiv.innerHTML = "Word not found";
                } else {
                    let meaning = data[0].meanings[0].definitions[0].definition;
                    let phonetics = data[0].phonetics.length ? data[0].phonetics[0].text : "N/A";
                    let audio = data[0].phonetics.length && data[0].phonetics[0].audio ? `<button class='audio-btn' onclick='playAudio("${data[0].phonetics[0].audio}")'>🔊 Play</button>` : "";
                    let example = data[0].meanings[0].definitions[0].example || "No example available";
                    resultDiv.innerHTML = `<h3>${word}</h3><p><strong>Phonetics:</strong> ${phonetics}</p>${audio}<p><strong>Meaning:</strong> ${meaning}</p><p><strong>Example:</strong> ${example}</p>`;
                }
            } catch (error) {
                resultDiv.innerHTML = "Error fetching data";
            }
        }
        function playAudio(url) {
            let audio = new Audio(url);
            audio.play();
        }
    </script>
</body>
</html>
