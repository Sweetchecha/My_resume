<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Python Интерпретатор</title>
    <style>
        body {
            font-family: 'Courier New', Courier, monospace;
            color: #00ff00;
            background-color: #000;
            margin: 0;
            padding: 0;
            overflow: hidden;
        }

        .matrix-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: black;
            overflow: hidden;
        }

        .content {
            position: relative;
            z-index: 1;
            padding: 20px;
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-out forwards;
        }

        textarea {
            width: 100%;
            height: 200px;
            font-family: monospace;
            font-size: 16px;
            color: #00ff00;
            background-color: #111;
            border: 1px solid #00ff00;
            margin-bottom: 20px;
            padding: 10px;
            box-sizing: border-box;
        }

        button {
            background-color: #00ff00;
            color: #000;
            font-size: 16px;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            margin-bottom: 20px;
        }

        button:hover {
            background-color: #00cc00;
        }

        #output {
            width: 100%;
            height: 200px;
            font-family: monospace;
            font-size: 16px;
            color: #00ff00;
            background-color: #111;
            border: 1px solid #00ff00;
            padding: 10px;
            box-sizing: border-box;
            overflow-y: auto;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <div class="matrix-bg" id="matrix"></div>
    <div class="content">
        <h1>Онлайн интерпретатор Python</h1>
        <textarea id="python-code">print("Добро пожаловать в Матрицу!")</textarea>
        <br>
        <button onclick="runPython()">Запустить</button>
        <div id="output"></div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/skulpt@1.2.0/skulpt.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/skulpt@1.2.0/skulpt-stdlib.js"></script>
    <script>
        function builtinRead(x) {
            if (Sk.builtinFiles === undefined || Sk.builtinFiles["files"][x] === undefined) {
                throw "File not found: '" + x + "'";
            }
            return Sk.builtinFiles["files"][x];
        }

        function runPython() {
            const code = document.getElementById("python-code").value;
            const outputElement = document.getElementById("output");
            outputElement.innerHTML = ""; // Очистка вывода

            Sk.configure({
                output: function(text) {
                    outputElement.innerHTML += text + "<br>";
                },
                read: builtinRead
            });

            Sk.importMainWithBody("<stdin>", false, code).catch(function(err) {
                outputElement.innerHTML = `<span style="color: red;">Ошибка: ${err}</span>`;
            });
        }

        // Matrix background
        const canvas = document.createElement('canvas');
        document.getElementById('matrix').appendChild(canvas);

        const ctx = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;

        const fontSize = 16;
        const columns = canvas.width / fontSize;
        const drops = Array(Math.floor(columns)).fill(1);
        const matrixChars = '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz';

        function drawMatrix() {
            ctx.fillStyle = 'rgba(0, 0, 0, 0.05)';
            ctx.fillRect(0, 0, canvas.width, canvas.height);

            ctx.fillStyle = '#0f0';
            ctx.font = `${fontSize}px monospace`;

            for (let i = 0; i < drops.length; i++) {
                const char = matrixChars[Math.floor(Math.random() * matrixChars.length)];
                const x = i * fontSize;
                const y = drops[i] * fontSize;
                ctx.fillText(char, x, y);

                if (y > canvas.height && Math.random() > 0.975) {
                    drops[i] = 0;
                }

                drops[i]++;
            }
        }

        setInterval(drawMatrix, 33);
    </script>
</body>
</html>
