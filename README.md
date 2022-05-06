# conversao-distancia

=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*

PROCEDIMENTOS PARA CRIAÇÃO DE IMAGEM E EXECUÇÃO DE CONTAINER

1º) Criar o documento "Dockerfile" para documentar a criação da imagem da aplicação

2º)Executar comando para a criação da imagem, criando as versões seguindo as boas práticas

      docker build -t felipejm91/conversao-distancia .
  
      docker build -t felipejm91/conversao-distancia:v1 .
 
3º)Executar comando para criação do container utilizando a imagem criada
  
      docker run -d --name conversao -p 8080:5000 felipejm91/conversao-distancia:v1
  
4º)Acessar a aplicação
  
      Abrir um navegador e digitar o caminho "localhost:8080"
  
5º)Aplicação rodando em container