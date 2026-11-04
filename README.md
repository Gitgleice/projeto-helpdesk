# projeto-helpdesk
desafio SQL
# Portfólio de Dados

Projetos e desafios de análise de dados com SQL.

## Projeto: Análise de Dados de Helpdesk

### Sobre o projeto

Este projeto simula uma operação de suporte técnico de uma empresa de tecnologia. O objetivo é estruturar um banco de dados relacional para analisar o histórico de chamados, identificar gargalos operacionais e propor melhorias para o negócio.

### Tecnologias e conceitos

- **Banco de dados:** MySQL
- Criação de tabelas e relacionamentos com chaves estrangeiras (DDL)
- Inserção de dados sintéticos (DML)
- Cruzamento de dados com `INNER JOIN`
- Agrupamentos com `GROUP BY`
- Agregações com `COUNT` e `AVG`
- Cálculo do tempo de resolução com `TIMESTAMPDIFF`

### Estrutura do banco de dados

O modelo contém três tabelas principais:

- **Analistas:** dados da equipe técnica.
- **Clientes:** empresas que abriram chamados.
- **Chamados:** registros dos tickets, incluindo datas de abertura e fechamento, prioridade, status e categoria.

### Perguntas de negócio

As consultas em [`queries.sql`](./queries.sql) respondem:

1. Quais categorias de problemas geram mais chamados?
2. Qual é o tempo médio de resolução, em minutos, por categoria?
3. Como os chamados estão distribuídos entre os analistas N1 e N2?

### Principais insights e recomendações

- **Problemas de senha** representam um volume alto de chamados, mas são resolvidos rapidamente (em menos de 30 minutos). **Recomendação:** implementar um sistema de autoatendimento para reduzir a demanda sobre a equipe de suporte.
- **Erros no sistema (bugs)** concentram os maiores tempos de espera e criticidade. **Recomendação:** fortalecer o alinhamento entre suporte e desenvolvimento para agilizar a investigação e a correção dos problemas.
