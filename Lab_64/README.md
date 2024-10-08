# Lab 64

# Projeto: Simulação de Upload via POST

## O que é isso?

Este projeto é uma simples simulação de upload de arquivos.
Nada muito complicado: você manda um arquivo através de uma requisição POST, e o servidor te responde com um "Upload simulado com sucesso!"
rodando na porta 3000.

## Como isso funciona?

Criando um servidor usando **Express**.
A rota principal é a `/upload`, e tudo o que essa rota faz é pegar o arquivo que você mandar e devolver uma mensagem de sucesso.

### Rotas principais:

- `/` - Página inicial
- `/about` - Página sobre nós
- `/upload` - Rota para enviar arquivos
- 404 - Rota de erro caso você erre o endereço

## Tecnologias usadas:

- **Node.js**
- **Express.js**
- **CORS**
- **Body-parser**

## Como rodar o projeto?

1. Clona esse repositório:
   ```bash
   git clone https://github.com/seu_usuario/seu_repositorio.git
   ```
2. Instale as dependencias:
   ```
   npm install
   ```
3. Rode o servidor:
   ```
   node server.js
   ```
4. Teste as urls:
   ```
   Para acessar a pagina principal: curl http://localhost:3000/
   ```
   ```
   Para acessar a pagina About: curl http://localhost:3000/about
   ```
   ```
   Para acessar a pagina 404: curl http://localhost:3000/algumaCoisa
   ```
   ```
   Para testar o envio de um arquivo: curl -X POST -F "file=@/caminho/para/seu/arquivo.txt" http://localhost:3000/upload
   ```
--------------- OU---------------
acessa as urls diretamente pelo navegador.  
