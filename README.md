<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trabalho de HTML</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
            line-height: 1.6;
            text-align: center;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        button {
            background: #007BFF;
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            border-radius: 5px;
            font-size: 16px;
        }
        button:hover {
            background: #0056b3;
        }
        form {
            display: flex;
            flex-direction: column;
            gap: 10px;
            margin-top: 20px;
        }
        input, textarea {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 16px;
            width: 100%;
        }
        textarea {
            height: 100px;
            resize: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1 id="title">Bem-vindo ao Trabalho de HTML</h1>
        <p id="description">Este site é sobre o trabalho de ajustes em HTML</p>
        <button id="changeText" times-new-roman="Mudar o texto da página">Mudar Texto</button>
        
        <form id="questionario">
            <label for="nome">Nome:</label>
            <input type="text" id="nome" name="nome" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="mensagem">Mensagem:</label>
            <textarea id="mensagem" name="mensagem" required></textarea>
            
            <button type="submit">Enviar</button>
        </form>
    </div>
    <script>
        document.getElementById('changeText').addEventListener('click', function() {
            document.getElementById('title').textContent = 'Texto Alterado com Sucesso!';
            document.getElementById('description').textContent = 'Agora você vê um novo texto na tela!';
        });
    </script>
</body>
</html>
