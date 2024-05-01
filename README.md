# ActiveMQ MuleSoft Integration

Este projeto de integração MuleSoft demonstra como integrar o ActiveMQ com diferentes endpoints utilizando o Mule 4.

## Configurações

### Dependências do MuleSoft

- Mule 4
- MuleSoft Anypoint Studio

### Configurações do ActiveMQ

- Broker URL: `tcp://localhost:61616`
- Username: `<your_username>`
- Password: `<your_password>`

### Configurações do Banco de Dados (MySQL)

- URL: `jdbc:mysql://localhost:3306/db_name`
- Username: `<your_username>`
- Password: `<your_password>`

## Fluxos Principais

### activeMQMysqlModeFlow

Este fluxo recebe mensagens do ActiveMQ e insere os dados em uma tabela do MySQL.

### activemq-moduleFlow

Este fluxo expõe um endpoint HTTP que transforma e publica mensagens no ActiveMQ.

### queue-subscriberFlow

Este fluxo consome mensagens de uma fila específica do ActiveMQ e exibe o payload no console.

### topic-subscriber

Este fluxo consome mensagens de um tópico específico do ActiveMQ e exibe o payload no console.

### activeMQ-RequestReplyFlow

Este fluxo recebe uma mensagem, a publica em uma fila do ActiveMQ e aguarda por uma resposta em outra fila.

### Request-Reply-Producer

Este fluxo consome mensagens de uma fila do ActiveMQ e exibe o payload no console como parte de um fluxo de solicitação-resposta.

## Como Executar

1. Clone o repositório.
2. Importe o projeto no Anypoint Studio.
3. Configure as conexões do ActiveMQ e do banco de dados MySQL.
4. Execute o projeto no Anypoint Studio.


---

Lembre-se de substituir `<your_username>` e `<your_password>` pelas suas credenciais reais. Este README fornece uma visão geral do projeto e ajuda os usuários a entender como ele funciona e como podem configurá-lo e executá-lo.
