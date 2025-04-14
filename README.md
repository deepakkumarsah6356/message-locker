<!DOCTYPE html>
<html>
<head>
    <title>Message Locker</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            padding: 30px;
            background-color: #f5f5f5;
        }

        input, textarea, button {
            margin: 10px 0;
            padding: 10px;
            width: 100%;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }

        #codeDisplay {
            background: #eee;
            padding: 10px;
            margin-top: 10px;
            border-radius: 4px;
        }

        footer {
            text-align: center;
            font-size: 12px;
            color: #aaa;
            margin-top: 30px;
        }

        .credit {
            text-align: right;
            font-style: italic;
            color: #888;
            font-size: 14px;
            margin-bottom: -10px;
        }
    </style>
</head>
<body>

    <p class="credit">by <b>deepakkumarsah_01</b></p>

    <h2>Secret Message Box</h2>

    <textarea id="messageInput" placeholder="Apna message likho..."></textarea>
    <button onclick="generateCode()">Submit</button>

    <div id="codeDisplay" style="display:none;">
        Aapka Unique Code: <b id="generatedCode"></b>
    </div>

    <hr>

    <input type="text" id="codeInput" placeholder="Code yahan daalein...">
    <button onclick="getMessage()">Message Dekhein</button>

    <div id="retrievedMessage" style="margin-top:20px;"></div>

    <footer>Made with love by deepakkumarsah_01</footer>

    <script>
        const messageStore = {};

        function generateCode() {
            const message = document.getElementById("messageInput").value.trim();
            if (!message) {
                alert("Pehle message likho!");
                return;
            }

            const code = Math.random().toString(36).substr(2, 8); // 8-char unique code
            messageStore[code] = message;

            document.getElementById("generatedCode").innerText = code;
            document.getElementById("codeDisplay").style.display = "block";
            document.getElementById("messageInput").value = '';
        }

        function getMessage() {
            const code = document.getElementById("codeInput").value.trim();
            const message = messageStore[code];

            const resultDiv = document.getElementById("retrievedMessage");
            if (message) {
                resultDiv.innerHTML = `<b>Message:</b> ${message}`;
            } else {
                resultDiv.innerHTML = `<span style="color:red;">Invalid ya expired code!</span>`;
            }
        }
    </script>
</body>
</html><!DOCTYPE html>
<html>
<head>
    <title>Message Locker</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            padding: 30px;
            background-color: #f5f5f5;
        }

        input, textarea, button {
            margin: 10px 0;
            padding: 10px;
            width: 100%;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }

        #codeDisplay {
            background: #eee;
            padding: 10px;
            margin-top: 10px;
            border-radius: 4px;
        }

        footer {
            text-align: center;
            font-size: 12px;
            color: #aaa;
            margin-top: 30px;
        }

        .credit {
            text-align: right;
            font-style: italic;
            color: #888;
            font-size: 14px;
            margin-bottom: -10px;
        }
    </style>
</head>
<body>

    <p class="credit">by <b>deepakkumarsah_01</b></p>

    <h2>Secret Message Box</h2>

    <textarea id="messageInput" placeholder="Apna message likho..."></textarea>
    <button onclick="generateCode()">Submit</button>

    <div id="codeDisplay" style="display:none;">
        Aapka Unique Code: <b id="generatedCode"></b>
    </div>

    <hr>

    <input type="text" id="codeInput" placeholder="Code yahan daalein...">
    <button onclick="getMessage()">Message Dekhein</button>

    <div id="retrievedMessage" style="margin-top:20px;"></div>

    <footer>Made with love by deepakkumarsah_01</footer>

    <script>
        const messageStore = {};

        function generateCode() {
            const message = document.getElementById("messageInput").value.trim();
            if (!message) {
                alert("Pehle message likho!");
                return;
            }

            const code = Math.random().toString(36).substr(2, 8); // 8-char unique code
            messageStore[code] = message;

            document.getElementById("generatedCode").innerText = code;
            document.getElementById("codeDisplay").style.display = "block";
            document.getElementById("messageInput").value = '';
        }

        function getMessage() {
            const code = document.getElementById("codeInput").value.trim();
            const message = messageStore[code];

            const resultDiv = document.getElementById("retrievedMessage");
            if (message) {
                resultDiv.innerHTML = `<b>Message:</b> ${message}`;
            } else {
                resultDiv.innerHTML = `<span style="color:red;">Invalid ya expired code!</span>`;
            }
        }
    </script>
</body>
</html><!DOCTYPE html>
<html>
<head>
    <title>Message Locker</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            padding: 30px;
            background-color: #f5f5f5;
        }

        input, textarea, button {
            margin: 10px 0;
            padding: 10px;
            width: 100%;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }

        #codeDisplay {
            background: #eee;
            padding: 10px;
            margin-top: 10px;
            border-radius: 4px;
        }

        footer {
            text-align: center;
            font-size: 12px;
            color: #aaa;
            margin-top: 30px;
        }

        .credit {
            text-align: right;
            font-style: italic;
            color: #888;
            font-size: 14px;
            margin-bottom: -10px;
        }
    </style>
</head>
<body>

    <p class="credit">by <b>deepakkumarsah_01</b></p>

    <h2>Secret Message Box</h2>

    <textarea id="messageInput" placeholder="Apna message likho..."></textarea>
    <button onclick="generateCode()">Submit</button>

    <div id="codeDisplay" style="display:none;">
        Aapka Unique Code: <b id="generatedCode"></b>
    </div>

    <hr>

    <input type="text" id="codeInput" placeholder="Code yahan daalein...">
    <button onclick="getMessage()">Message Dekhein</button>

    <div id="retrievedMessage" style="margin-top:20px;"></div>

    <footer>Made with love by deepakkumarsah_01</footer>

    <script>
        const messageStore = {};

        function generateCode() {
            const message = document.getElementById("messageInput").value.trim();
            if (!message) {
                alert("Pehle message likho!");
                return;
            }

            const code = Math.random().toString(36).substr(2, 8); // 8-char unique code
            messageStore[code] = message;

            document.getElementById("generatedCode").innerText = code;
            document.getElementById("codeDisplay").style.display = "block";
            document.getElementById("messageInput").value = '';
        }

        function getMessage() {
            const code = document.getElementById("codeInput").value.trim();
            const message = messageStore[code];

            const resultDiv = document.getElementById("retrievedMessage");
            if (message) {
                resultDiv.innerHTML = `<b>Message:</b> ${message}`;
            } else {
                resultDiv.innerHTML = `<span style="color:red;">Invalid ya expired code!</span>`;
            }
        }
    </script>
</body>
</html>
