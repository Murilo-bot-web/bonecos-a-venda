<!DOCTYPE html><html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Super Produto Exclusivo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: white;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .container {
            border-left: 5px solid blue;
            border-right: 5px solid black;
            padding: 20px;
            max-width: 400px;
            margin-top: 50px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        img {
            width: 100%;
            height: auto;
        }
        .price {
            font-size: 24px;
            color: black;
            margin: 10px 0;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            background-color: blue;
            color: white;
            border: none;
            cursor: pointer;
            margin-top: 10px;
        }
        button:hover {
            background-color: darkblue;
        }
        .error-box {
            display: none;
            margin-top: 20px;
            padding: 15px;
            border: 1px solid black;
            background-color: #f8f8f8;
            text-align: center;
        }
        .error-title {
            color: red;
            font-size: 20px;
            font-weight: bold;
        }
        .error-message {
            color: black;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Super Produto Exclusivo</h1>
        <img src="/mnt/data/file-KRkGQYtjVdF6LVS4aLJUmp" alt="Produto">
        <p class="price">R$ 32,00</p>
        <button onclick="mostrarErro()">Comprar</button>
        <div class="error-box" id="erro">
            <p class="error-title">ERRO</p>
            <p class="error-message">O estoque já se esgotou, lamento.</p>
        </div>
    </div>
    <script>
        function mostrarErro() {
            document.getElementById("erro").style.display = "block";
        }
    </script>
</body>
</html>
