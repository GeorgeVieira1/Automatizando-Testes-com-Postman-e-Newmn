# Automatizando-Testes-com-Postman-e-Newmn
Criar um cenário de testes para testar uma API (Hunter)
>Criar um projeto no Postman para verificar a saúde dos recursos dessa API, rodando um conjunto de testes de forma automática.
>
>---
### Tipos de testes 🤖

- Teste funcional Para os testes , foi criado um xlsx com o planejamento dos testes, com detalhamento de cenários de testes, passos e resultado esperado
- API: Para os testes de api, foi criada uma duas collections no Postman e utilizando o ambiente `Tests`, foi criado casos de teste. A collection está estruturada com Casos de Teste de sucesso e exceção, cobrindo as funcionalidades do

- ---
### Casos de testes📍
📄 Validar o método POST
- [x] Criar novo lead

📄 Validar o método GET
- [x] Recuperar todos leads cadastrados
- [x] Recuperar lead específico

📄 Validar o método PUT
- [x] Editar lead

📄 Validar o método DELETE
- [x] Excluir lead

- ---
### Executando os testes ⚙️
⚙️Foi realizado o método POST onde foi criado um novo lead, o teste teve retorno 201 onde houve uma validação de retorno.
Resultado esperado:
 Status code: 200, 201 ou 202;
- String 'Created' no status code do response;
- Tempo de execução < 2 seg.
  
  ![image](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/bb531f2b-4be3-4de8-ac40-7cb81c9e2dde)

⚙️Foi realizado o método GET Recuperar lead específico, Enviar requisição GET assíncrona para recuperar todos os leads, o teste teve retorno 200 onde houve uma validação de retorno.
Resultado esperado:
- Status code: 200;
- String 'OK' no status code do response;
- Tempo de execução < 2 seg
  
![image](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/4ebded8d-507b-4671-a122-889a083ce15f)
![image](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/0d9b7613-e446-40bd-a391-d2a0ced3d27e)










