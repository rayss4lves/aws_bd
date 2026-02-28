# aws_bd
RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS
Data: 27 de Fevereiro de 2026

Empresa: Abstergo Industries

Responsável: Rayssa

Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Rayssa. O objetivo do projeto foi elencar 3 serviços AWS com a finalidade de realizar a diminuição de custos imediatos e otimizar a utilização de recursos em nuvem.

Descrição do Projeto
O projeto foi dividido em 3 etapas estratégicas:

Etapa 1: Armazenamento Inteligente de Objetos

Ferramenta: Amazon S3 Intelligent-Tiering.

Foco da ferramenta: Automação de custos de armazenamento.

Descrição de caso de uso: Implementado para os arquivos de mídia e backups da Abstergo. A ferramenta utiliza Machine Learning para mover automaticamente arquivos não acessados para camadas mais baratas, eliminando o pagamento por armazenamento "quente" em dados que não são utilizados frequentemente.

Etapa 2: Banco de Dados de Alto Desempenho e Escalabilidade

Ferramenta: Amazon Aurora (com instâncias Serverless v2).

Foco da ferramenta: Redução de custos de infraestrutura e licenciamento.

Descrição de caso de uso: Migração dos bancos de dados MySQL/PostgreSQL para o Aurora. O uso do modo Serverless permite que o banco diminua sua capacidade (e custo) para quase zero em períodos de baixa demanda, evitando gastos com servidores ociosos durante a madrugada ou finais de semana.

Etapa 3: Cache de Performance para NoSQL

Ferramenta: Amazon DynamoDB Accelerator (DAX).

Foco da ferramenta: Redução de consumo de IOPS (RCU).

Descrição de caso de uso: Adição de uma camada de cache em memória para as tabelas de alta leitura do DynamoDB. Ao responder requisições em microssegundos através do cache, reduzimos a necessidade de provisionar unidades de leitura caras no banco de dados principal, gerando economia direta na fatura mensal.

Conclusão
A implementação das ferramentas na empresa Abstergo Industries tem como esperado a redução de até 30% nos custos mensais de infraestrutura, além de aumentar a eficiência e a produtividade da equipe de TI através da automação. Recomenda-se a continuidade da utilização das ferramentas e o monitoramento via AWS Cost Explorer para validar as projeções