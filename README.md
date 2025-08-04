# btg-pactual-order-processor

Desafio técnico para a vaga de Engenheiro de Software no BTG Pactual.

## 📌 Objetivo
Criar uma aplicação que consome pedidos via fila RabbitMQ, persiste os dados no MongoDB e expõe uma API REST com relatórios e informações agregadas.

## ⚙️ Tecnologias Utilizadas
- Java 21
- Spring Boot
- MongoDB
- RabbitMQ
- Docker
- TDD com JUnit 5 e Mockito

## 📁 Estrutura Inicial

- Modelagem de domínio com as classes `Pedido` e `Item`, representando os dados reais dos pedidos
- Testes unitários com TDD cobrindo:
  - Cálculo do valor total do pedido
  - Cenário de lista de itens vazia
  - Pedido com um item
  - Cenário com valores inesperados (como quantidades negativas)
- API REST com Spring Boot (em desenvolvimento)
- Microserviço consumidor RabbitMQ (em desenvolvimento)
- Banco MongoDB com repositório dos pedidos
- Ambiente dockerizado (em breve)

## ✅ Funcionalidades Implementadas

- Cálculo do valor total de pedidos com base em itens (quantidade x preço unitário)
- Testes automatizados com JUnit 5 garantindo a consistência da lógica de domínio
- Repositório com Spring Data MongoDB para persistência
- Código estruturado com boas práticas em pacotes separados: `model`, `repository`, `config`, `service`

## 🚀 Como executar
(Instruções futuras de como rodar via Docker e testar)

## 📌 Autor
[Isaque-Br](https://github.com/Isaque-Br)
