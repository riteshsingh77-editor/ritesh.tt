# ritesh.tt
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I'm Sorry, My Love</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fce4ec;
            text-align: center;
        }
        header {
            background-color: #ff80ab;
            color: white;
            padding: 30px 20px;
        }
        header h1 {
            margin: 0;
            font-size: 3rem;
        }
        header p {
            font-size: 1.2rem;
            margin-top: 10px;
        }
        section {
            padding: 50px 20px;
        }
        h2 {
            color: #d81b60;
            font-size: 2.5rem;
        }
        p {
            font-size: 1.2rem;
            color: #880e4f;
        }
        .heart {
            font-size: 5rem;
            color: #d81b60;
            margin: 20px 0;
            animation: heartbeat 1s infinite;
        }
        @keyframes heartbeat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }
        .button {
            display: inline-block;
            margin-top: 20px;
            padding: 15px 30px;
            font-size: 1.2rem;
            color: white;
            background-color: #d81b60;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        .button:hover {
            background-color: #c2185b;
        }
        #sorry-container {
            display: none;
            margin-top: 30px;
        }
        .sorry-text {
            font-size: 1.2rem;
            color: #d81b60;
            margin: 5px 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>I'm Sorry, My Love</h1>
        <p>I hope you can forgive me...</p>
    </header>
    <section>
        <h2>My Love,</h2>
        <p>I know I made a mistake, and I feel truly sorry from the bottom of my heart.</p>
        <p>You mean the world to me, and I can't bear the thought of losing you.</p>
        <div class="heart">❤️</div>
        <p>Please forgive me and give me a chance to make things right. I promise to cherish you and make you smile forever.</p>
        <button class="button" onclick="showSorry()">Click Here If You Forgive Me</button>
        <div id="sorry-container"></div>
    </section>

    <script>
        function showSorry() {
            const container = document.getElementById('sorry-container');
            container.style.display = 'block';
            container.innerHTML = ''; // Clear previous content if clicked again

            for (let i = 0; i < 100; i++) {
                const sorryText = document.createElement('div');
                sorryText.className = 'sorry-text';
                sorryText.textContent = 'Sorry 💖';
                container.appendChild(sorryText);
            }
        }
    </script>
</body>
</html>
