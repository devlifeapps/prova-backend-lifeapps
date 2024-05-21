<p align="center">
    <img src="https://i.ytimg.com/vi/myJ_Darr0ng/maxresdefault.jpg" alt="Lifeapps" style="width:60%"/>
</p>


# 💻 Desafio Backend Lifeapps

Olá candidato(a). Este é o desafio frontend da Lifeapps!

Sinta-se à vontade para perguntar qualquer coisa que não esteja claro, mas lembre-se: o desafio é individual!
Quando terminar, responda o email com o link do seu repositório.
Nosso time de engenharia irá avaliar o seu código e entrará em contato com você.

Tenha em mente que o desafio é uma oportunidade para você mostrar suas habilidades e conhecimentos em desenvolvimento backend. Portanto, capriche! 🚀

> ⚠️ **É importante que o seu repositório esteja público, caso contrário não iremos conseguir avaliar sua resposta**

# 📈 Objetivo: Microsserviços para E-commerce

Este desafio técnico destina-se a candidatos para a vaga de Desenvolvedor Backend Node.js na nossa empresa de e-commerce. O objetivo é avaliar a compreensão de sistemas distribuídos entre microsserviços, bem como a preocupação com a qualidade do código.

## Contexto

Você foi contratado por uma empresa de e-commerce para desenvolver uma solução de microsserviços que permita atender de maneira escalável a efetivação de seus pedidos sem prejudicar o controle do estoque dos produtos. 
Sua missão é criar duas aplicações que se comuniquem de forma assíncrona e persistam informações relacionadas a pedidos de clientes e inventário de produtos.

## Desafio

Você deve criar duas aplicações:

1. **Serviço de Pedidos (Order Service):** Este serviço será responsável por receber pedidos de clientes e persistir as informações relacionadas aos pedidos em um banco de dados. Ele deve ser capaz de se comunicar assíncronamente com o segundo serviço para atualizar o inventário de produtos após a realização de um pedido.

4. **Serviço de Inventário (Inventory Service):** Este serviço será responsável por gerenciar o inventário de produtos disponíveis para venda. Ele deve ser capaz de receber mensagens assíncronas do Serviço de Pedidos para atualizar o inventário sempre que um pedido for feito.

## Exemplos de API

### Endpoint para Inserção de Pedido

POST /api/orders

**Corpo da Requisição:**
```json
{
  "customer_id": "123456",
  "products": [
    {
      "product_id": "789",
      "quantity": 2,
      "price": 19.99
    },
    {
      "product_id": "456",
      "quantity": 1,
      "price": 29.99
    }
  ]
}
```

**Resposta da Requisição (Exemplo de Resposta 200 OK):**

```json
{
  "order_id": "987654",
  "status": "received",
  "message": "Order successfully placed."
}
```

# 🔍 Observações
- Os serviços devem se comunicar de forma assíncrona, garantindo a integridade dos dados em caso de falha.
- Os serviços devem ser desenvolvidos com foco na legibilidade, modularidade e reutilização de código.
- Deve ser implementada uma estratégia de tratamento de falhas que garanta a disponibilidade do sistema mesmo em situações de falha parcial.
- É fundamental seguir boas práticas de desenvolvimento e padrões de projeto.
- Será considerado um diferencial o desenvolvimento de testes unitários para a cobertura do código desenvolvido.

# 🗂️ Requisitos

- A linguagem utilizada deve ser **Node.js**
- O repositório deve conter os arquivos Docker necessários para executar a aplicação.
- Deve ser utilizado banco de dados (Relacional ou NoSQL) para persistência das transações.
- A arquitetura da solução deve estar documentada da forma desejada pelo candidato.

# 💎 Entrega e Feedback

Você terá 7 dias para completar o desafio. Após a entrega, será agendada uma entrevista técnica para discutir as soluções adotadas por você. Durante essa entrevista, abordaremos possíveis cenários reais de escalabilidade e falha no sistema, além de revisar o código desenvolvido.

Boa sorte!
