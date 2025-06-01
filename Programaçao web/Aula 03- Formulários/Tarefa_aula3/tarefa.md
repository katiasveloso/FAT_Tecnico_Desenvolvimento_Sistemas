# Tarefa
## Para Pensar e Responder

Os formulários são excelentes ferramentas para receber dúvidas, sugestões e críticas, pesquise sites onde você pode visualizar as informações e tente criar um código em html para apresentar os formulários.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fórmularios</title>
</head>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #f4f4f4;
        margin: 0;
        padding: 30px;
    }

    h1 {
        text-align: center;
        color: #333;
    }

    form {
        max-width: 600px;
        margin: auto;
        background-color: #fff;
        padding: 20px;
        border-radius: 5px;
        box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    }

    label {
        display: block;
        margin-bottom: 8px;
    }

    input[type="text"],
    input[type="email"],
    input[type="password"],
    select,
    textarea {
        width: calc(100% - 20px);
        padding: 10px;
        margin-bottom: 15px;
        border-radius: 5px;
        border: 1px solid #ccc;
    }

    input[type="submit"] {
        background-color: #28a745;
        color: white;
        border: none;
        padding: 10px 15px;
        cursor: pointer;
        border-radius: 5px;
    }

    input[type="submit"]:hover {
        background-color: #218838;
    }
   
</style>


<body>
   <h1 style="color: blue;">Fórmularios</h1>
    <form action="inscrição.php" method="post">
        <label for="nome">Nome:</label>
        <input type="text" id="nome" name="nome" required>
        <br><br>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
        <br><br>

        <label for="senha">Senha:</label>
        <input type="password" id="senha" name="senha" required>
        <br>
            <h4>Selecione o curso:</h4>
        <select id="curso" name="curso" label ="Selecione o curso" required>
            <option value="programacao">Programação</option>
            <option value="design">Design</option>
            <option value="marketing">Marketing</option>
        </select>
        <br><br>
        
        <div>
            <label for ="mensagem">Mensagem:</label><br>
            <textarea id="mensagem" name="mensagem" rows="5" cols="50" placeholder="Escreva sua mensagem aqui..."></textarea>
        </div>


        <input type="submit" value="Enviar">

    
</body>
</html>

```