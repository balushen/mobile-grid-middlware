_____________________________________________________________________________
v0.1

Funcionamento:
- Resource � um recurso na rede e espera por requisi��es na porta 12399
- Broker conecta e envia um objeto GridJob para ser executado
- Resource executa e envia a resposta
- 1 Conex�o do Broker envia 1 lista de Jobs para executar
- 1 Conex�o de resposta do Resource envia uma lista de resposta ordenados respectivamente a cada job

Para utilizar o Middleware:
- Criar objetos GridJob que ser�o distribuidos no grid
- Utilizar o m�todo dispatchJobs da classe Broker para enviar os Jobs e aguardar a resposta
- Se n�o houver exce��es utilizar o m�todo getReplies para receber as resopstas na ordem enviada
_____________________________________________________________________________
