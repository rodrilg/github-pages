<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Cadastro para Recurso de Multa</title>
</head>
<body>

<h2>Cadastro de Dados para Recurso de Multa</h2>
<p>Preencha seus dados e envie uma imagem da sua CNH para darmos início à elaboração do seu recurso.</p>

<form action="/enviar-dados" method="POST" enctype="multipart/form-data">
  
  <label for="nome">Nome completo:</label><br>
  <input type="text" id="nome" name="nome" required><br><br>

  <label for="cpf">CPF:</label><br>
  <input type="text" id="cpf" name="cpf" pattern="\d{3}\.\d{3}\.\d{3}-\d{2}" placeholder="000.000.000-00" required><br><br>

  <label for="numero_cnh">Número da CNH:</label><br>
  <input type="text" id="numero_cnh" name="numero_cnh" required><br><br>

  <label for="foto_cnh">Upload da CNH (imagem):</label><br>
  <input type="file" id="foto_cnh" name="foto_cnh" accept=".jpg,.jpeg,.png,.pdf" required><br><br>

  <h3>Informações de contato (opcional)</h3>

  <label for="telefone">Telefone:</label><br>
  <input type="tel" id="telefone" name="telefone" pattern="\(\d{2}\)\s?\d{4,5}-\d{4}" placeholder="(00) 00000-0000"><br><br>

  <label for="email">E-mail:</label><br>
  <input type="email" id="email" name="email"><br><br>

  <button type="submit">Enviar dados e CNH</button>

</form>

</body>
</html>
