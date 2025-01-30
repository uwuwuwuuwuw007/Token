
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TOKEN CHECKER</title>
    <link rel="stylesheet" href="/static/styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            max-width: 600px;
            width: 100%;
            background: white;
            padding: 30px;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
            border-radius: 8px;
            text-align: center;
        }

        h1 {
            color: #333;
            margin-bottom: 20px;
        }

        label {
            display: block;
            margin: 15px 0 5px;
            font-weight: bold;
            text-align: left;
        }

        input[type="text"], input[type="file"] {
            width: 100%;
            padding: 12px;
            margin-bottom: 20px;
            border-radius: 8px;
            border: 1px solid #ccc;
            box-sizing: border-box;
            font-size: 16px;
        }

        button {
            background-color: #28a745;
            color: white;
            padding: 12px 25px;
            border: none;
            cursor: pointer;
            border-radius: 8px;
            font-size: 16px;
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #218838;
        }

        #resultBox {
            margin-top: 30px;
            text-align: left;
        }

        ul {
            list-style: none;
            padding: 0;
        }

        ul li {
            background: #d4edda;
            padding: 10px;
            margin-bottom: 10px;
            border-radius: 8px;
        }

        #invalidTokenList li {
            background: #f8d7da;
        }

        #copyButton, #copyInvalidButton {
            margin-top: 10px;
            padding: 10px 20px;
            background-color: #007bff;
            border-radius: 8px;
        }

        #copyButton:hover, #copyInvalidButton:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>TOKEN CHECKER</h1>
        <form id="tokenForm">
            <label for="tokenInput">Enter Single Token:</label>
            <input type="text" id="tokenInput" name="single_token" placeholder="Enter token here">
            
            <label for="tokenFile">Or Upload Token File:</label>
            <input type="file" id="tokenFile" name="token_file">
            
            <button type="submit">Validate Tokens</button>
        </form>

        <div id="resultBox" style="display: none;">
            <h3>Validation Results</h3>
            <p>Total Tokens: <span id="totalTokens"></span></p>
            <p>Valid Tokens: <span id="validCount"></span></p>
            <p>Invalid Tokens: <span id="invalidCount"></span></p>

            <h4>Valid Tokens:</h4>
            <ul id="validTokenList"></ul>

            <h4>Invalid Tokens:</h4>
            <ul id="invalidTokenList"></ul>

            <button id="copyButton">Copy All Valid Tokens</button>
            <button id="copyInvalidButton">Copy All Invalid Tokens</button>
        </div>

        <script>
            document.getElementById('tokenForm').addEventListener('submit', function(e) {
                e.preventDefault();

                let formData = new FormData(this);

                fetch('/validate', {
                    method: 'POST',
                    body: formData
                })
                .then(response => response.json())
                .then(data => {
                    document.getElementById('totalTokens').innerText = data.total_tokens;
                    document.getElementById('validCount').innerText = data.valid_count;
                    document.getElementById('invalidCount').innerText = data.invalid_count;

                    let validList = document.getElementById('validTokenList');
                    let invalidList = document.getElementById('invalidTokenList');
                    validList.innerHTML = '';
                    invalidList.innerHTML = '';

                    data.valid_tokens.forEach(token => {
                        let li = document.createElement('li');
                        li.innerText = `Name: ${token.name}, ID: ${token.id}, Token: ${token.token}`;
                        validList.appendChild(li);
                    });

                    data.invalid_tokens.forEach(token => {
                        let li = document.createElement('li');
                        li.innerText = `Name: ${token.name}, ID: ${token.id}, Token: ${token.token}`;
                        invalidList.appendChild(li);
                    });

                    document.getElementById('resultBox').style.display = 'block';
                });
            });

            document.getElementById('copyButton').addEventListener('click', function() {
                let validTokens = document.querySelectorAll('#validTokenList li');
                let tokenText = Array.from(validTokens).map(li => li.innerText).join('\n');

                navigator.clipboard.writeText(tokenText)
                    .then(() => alert('Copied all valid tokens!'))
                    .catch(err => console.error('Failed to copy: ', err));
            });

            document.getElementById('copyInvalidButton').addEventListener('click', function() {
                let invalidTokens = document.querySelectorAll('#invalidTokenList li');
                let tokenText = Array.from(invalidTokens).map(li => li.innerText).join('\n');

                navigator.clipboard.writeText(tokenText)
                    .then(() => alert('Copied all invalid tokens!'))
                    .catch(err => console.error('Failed to copy: ', err));
            });
        </script>
    </div>
<script defer src="https://static.cloudflareinsights.com/beacon.min.js/vcd15cbe7772f49c399c6a5babf22c1241717689176015" integrity="sha512-ZpsOmlRQV6y907TI0dKBHq9Md29nnaEIPlkf84rnaERnq6zvWvPUqr2ft8M1aS28oN72PdrCzSjY4U6VaAw1EQ==" data-cf-beacon='{"rayId":"90a43a497c02edfe","version":"2025.1.0","r":1,"token":"dcaf3911e6af4adda295fea97d02aa44","serverTiming":{"name":{"cfExtPri":true,"cfL4":true,"cfSpeedBrain":true,"cfCacheStatus":true}}}' crossorigin="anonymous"></script>
</body>
</html>
