# 1. O Que Significa API 🧠

API = Application Programming Interface

Application → Programas, apps, serviços ou sistemas.

Programming → Interação feita via código ou requisições.

Interface → Um ponto de comunicação entre duas partes.

Ela funciona como um contrato 📜:

Quem envia a solicitação (request) deve seguir regras.

Quem responde (response) segue o mesmo padrão.

# 2. Como Uma API Funciona na Prática ⚙️

A comunicação geralmente acontece via HTTP (o mesmo protocolo dos sites).
O cliente (você) envia uma requisição → A API processa → O servidor devolve uma resposta.

Exemplo simples:

Queremos saber o clima em São Paulo usando a OpenWeather API.

GET https://api.openweathermap.org/data/2.5/weather?q=São%20Paulo&appid=SUA_CHAVE_API&units=metric&lang=pt_br

Resposta (JSON):
{
  "name": "São Paulo",
  "main": {
    "temp": 27.5,
    "humidity": 60
  },
  "weather": [
    {
      "description": "céu limpo"
    }
  ]
}


💡 O que aconteceu:

Fizemos um GET → pedimos informações.

A API consultou a base de dados.

Recebemos a resposta estruturada em JSON.

# 3. Componentes Básicos de uma API 🧩

| **Componente**   | **Função**                                         | **Exemplo**                      |
| ---------------- | -------------------------------------------------- | -------------------------------- |
| **Endpoint**     | Endereço onde o cliente acessa a API               | `/data/2.5/weather`              |
| **Método HTTP**  | Tipo de operação que será executada                | GET, POST, PUT, DELETE           |
| **Headers**      | Informações adicionais para autenticação e formato | `Content-Type: application/json` |
| **Parâmetros**   | Filtros ou dados extras enviados na URL            | `?q=São Paulo&lang=pt_br`        |
| **Request Body** | Dados enviados no corpo da requisição (POST)       | `{ "nome": "Paulo" }`            |
| **Response**     | Retorno da API, normalmente em JSON                | `{ "status": "ok" }`             |
| **Status Code**  | Código numérico indicando sucesso ou erro          | `200`, `401`, `404`, `500`       |


# 4. Tipos de APIs 🔄

| **Tipo**     | **Descrição**                                                | **Exemplo**                      |
| ------------ | ------------------------------------------------------------ | -------------------------------- |
| **REST**     | Baseada em recursos, usa HTTP e JSON. É a mais comum.        | OpenWeather, Telnyx, Google Maps |
| **SOAP**     | Usa XML e um protocolo mais rígido.                          | Sistemas bancários antigos       |
| **GraphQL**  | Permite pedir **exatamente** os dados que você quer.         | GitHub GraphQL API               |
| **Webhooks** | Ao invés de pedir, você **recebe notificações automáticas**. | Pagamentos no Stripe             |
| **gRPC**     | Usada para comunicação rápida entre microsserviços.          | Google, Netflix                  |


Para o seu aprendizado inicial, REST APIs são o principal foco.

# 5. Métodos HTTP Mais Usados 🌐

| **Método** | **Função**             | **Exemplo prático**       |
| ---------- | ---------------------- | ------------------------- |
| **GET**    | Buscar dados           | Buscar clima atual        |
| **POST**   | Enviar dados           | Criar novo usuário        |
| **PUT**    | Atualizar tudo         | Atualizar perfil completo |
| **PATCH**  | Atualizar parcialmente | Alterar só o e-mail       |
| **DELETE** | Remover dados          | Excluir conta             |


# 6. Códigos de Resposta da API (Status Codes) 🟢🔴

| **Código** | **Categoria**      | **Significado**              |
| ---------- | ------------------ | ---------------------------- |
| **200**    | ✅ Sucesso          | Tudo certo, resposta enviada |
| **201**    | ✅ Criado           | Novo recurso criado          |
| **400**    | ⚠️ Erro do cliente | Dados inválidos              |
| **401**    | 🔒 Não autorizado  | Falta de autenticação        |
| **404**    | ❌ Não encontrado   | Endpoint inexistente         |
| **500**    | 🔴 Erro interno    | Problema no servidor         |


# 7. Benefícios do Uso de APIs 🚀

**Automação** → Conecta ferramentas sem esforço manual.

**Escalabilidade** → Permite integrar novos sistemas rapidamente.

**Padronização** → Comunicação estruturada e previsível.

**Reuso** → Várias aplicações podem usar a mesma API.

**Produtividade** → Economiza tempo no desenvolvimento.

# 8. Exercício Prático para Fixar 🧠

Acesse o site JSONPlaceholder
.

Teste no navegador o endpoint:

https://jsonplaceholder.typicode.com/posts/1


Veja a resposta em JSON.

Agora, teste o mesmo endpoint no [Postman](https://github.com/pcfelias65-code/Automation/blob/Introdu%C3%A7%C3%A3o/0001a%20-%20Exerc%C3%ADcio%20PostMan.jpg) ou Insomnia.

Anote a diferença entre o GET pelo navegador e pelo Postman.

# Resumo Final 🏁

Uma API é como um garçom entre o cliente e a cozinha:

- Ela recebe pedidos estruturados.

- Entende o que você quer.

- Retorna exatamente os dados que você precisa.

Entender APIs é o primeiro passo para dominar automação, integração de sistemas e ferramentas como n8n.
Quanto mais você praticar, mais natural essa comunicação entre sistemas vai parecer.
