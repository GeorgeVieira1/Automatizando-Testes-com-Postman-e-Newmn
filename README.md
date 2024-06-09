# Automatizando-Testes-com-Postman-e-Newmn
Criar um cenário de testes para testar uma API (Hunter)
>Criar um projeto no Postman para verificar a saúde dos recursos dessa API, rodando um conjunto de testes de forma automática.

>---
### Tipos de testes 🤖

- Teste funcional: 🛞 Para os testes , foi criado um xlsx com o planejamento dos testes, com detalhamento de cenários de testes, passos e resultado esperado, segue o código para o plano de testes: [https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn.git](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/blob/main/plano%2Bde%2Btestes.xlsx).
- API: Para os testes de api, foi criada uma duas collections no Postman e utilizando o ambiente `Desenvolvimento`, foi criado casos de teste. A collection está estruturada com Casos de Teste de sucesso.
- Rodar os testes da API de forma automática via Runner.
- Executar via Newman a "Collection" e "environment" (Desenvolvimento) exportados.
- Relatório dos testes com newman.

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

- Status code: 200, 201 ou 202;
- String 'Created' no status code do response;
- Tempo de execução < 2 seg.
  
  ![image](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/bb531f2b-4be3-4de8-ac40-7cb81c9e2dde)


⚙️Enviar requisição GET assíncrona para recuperar todos os leads, o teste teve retorno 200 onde houve uma validação de retorno.

Resultado esperado:
- Status code: 200;
- String 'OK' no status code do response;
- Tempo de execução < 2 seg
  
![image](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/4ebded8d-507b-4671-a122-889a083ce15f)
![image](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/0d9b7613-e446-40bd-a391-d2a0ced3d27e)


⚙️Enviar requisição GET assíncrona para recuperar lead específico, o teste teve retorno 200 onde houve uma validação de retorno.


Resultado esperado:
- Status code: 200;
- String 'OK' no status code do response;
- Tempo de execução < 2 seg

![image](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/330b572b-d7ab-4651-b6e1-abfe759c63d3)


⚙️Enviar requisição PUT assincrona para alterar Lead, Foi alterado o e-amail, o nome e último nome, adiconado "editado" em cada um.
Resultado esperado:
- Status code: 204;
- String 'No Content' no response code.

![image](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/7aa85886-3133-4402-bde0-0d28e906e3cc)


⚙️Enviar requisição DELETE assincrona para deletar lead específico, todos excluídos com sucesso.

Resultado esperado:
- Status code: 204;
- String 'No Content' no response code.

![image](https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/e4cb388b-20b5-4649-a0b5-9ed71efcf2db)

- ---
### Executando os testes da API com Runner

https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/10bddef3-fb38-4185-9542-8154b06167ff

- ---
### Execução das collections  e ambientes exportados com o newman no prompt de comando:
☑️ Permite rodar as collections que foram exportadas do postman, utilizandos as variáveis presentes no ambiente de desevolvimento ou demais ambientes.


https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/5fd780eb-3abe-4d81-8408-7ebd4e94ea28

- ---
### Resultado relatório dos testes com newman: 
☑️ É uma ferramenta de linha de comendo para executar collections de testes de API.  Ele permite que você integre seus testes de API criados no Postman com pipelines de CI/CD e scripts de automação.


https://github.com/GeorgeVieira1/Automatizando-Testes-com-Postman-e-Newmn/assets/122054835/d1df0332-6741-4d7a-8a02-7324e4d62e89



  






