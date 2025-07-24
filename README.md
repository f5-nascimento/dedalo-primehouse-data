# Dédalo PrimeHouse Data

## Contextualização

A **Dédalo PrimeHouse**, empresa especializada na intermediação, administração e comercialização de imóveis residenciais e comerciais, identificou a necessidade de modernizar sua infraestrutura tecnológica. Suas operações estavam apoiadas em sistemas locais e planilhas, o que comprometia o acesso remoto, a integridade dos dados e a escalabilidade dos processos.

Para superar esses desafios, a Dédalo PrimeHouse contratou a **Orion Data Solutions**, empresa de tecnologia da informação com expertise em soluções de banco de dados e infraestrutura em nuvem. A missão foi atribuída à **Equipe Atlas**, um time especializado em arquitetura de dados e implementação de sistemas em ambientes escaláveis e seguros.

A proposta do projeto consiste na criação de uma base de dados relacional hospedada na nuvem, utilizando o serviço **Azure Database for PostgreSQL**, que será responsável por armazenar e gerenciar as informações essenciais do negócio — como dados de clientes, corretores, imóveis e vendas.

O trabalho desenvolvido pela Equipe Atlas envolve desde a criação do ambiente em nuvem até a estruturação das tabelas, inserção de dados simulados e desenvolvimento de consultas e visualizações que permitam à Dédalo PrimeHouse ter uma visão consolidada e estratégica de suas operações.

---
## Diagrama

<img width="843" height="374" alt="corretora - public - vendas" src="https://github.com/user-attachments/assets/be852147-c44e-420c-9dd2-3543ce77b540" />



---
## Instruções da Atividade

### Passo 01 - Criação do Servidor
Crie um servidor flexível no serviço **Azure Database for PostgreSQL**, que será utilizado para hospedar o banco de dados da corretora de imóveis.

### Passo 02 - Criação do Banco de Dados
No servidor criado, crie um banco de dados com o nome `corretora` para armazenar as tabelas e dados do sistema imobiliário.

### Passo 03 - Conexão com o Banco de Dados
Utilize a ferramenta cliente **DBeaver** para estabelecer uma conexão com o banco de dados `corretora`. Essa conexão deve permitir a execução de comandos SQL diretamente no servidor PostgreSQL hospedado no Azure.

### Passo 04 - Criação da Tabela Clientes
Crie a tabela `clientes` no banco `corretora` conforme o modelo lógico fornecido, definindo os campos, tipos de dados e restrições de integridade necessárias.

### Passo 05 - Inserção de Dados na Tabela Clientes
Utilize uma ferramenta de inteligência artificial para gerar um script SQL contendo, no mínimo, **100 registros válidos** para a tabela `clientes`. Execute esse script no banco de dados utilizando o DBeaver para popular a tabela com dados simulados.

### Passo 06 - Criação da Tabela Corretores
Crie a tabela `corretores` no banco `corretora` de acordo com o modelo lógico disponibilizado, garantindo que os atributos, tipos e restrições estejam adequados.

### Passo 07 - Inserção de Dados na Tabela Corretores
Insira pelo menos **10 registros** na tabela `corretores`, utilizando dados coerentes e realistas.

### Passo 08 - Criação da Tabela Imovel
Crie a tabela `imovel` no banco de dados `corretora`, conforme a estrutura definida no diagrama lógico da corretora de imóveis. Garanta que todos os atributos, tipos de dados e restrições de integridade estejam corretamente implementados.

### Passo 09 - Alteração da Tabela Imovel
Utilize o comando adequado para adicionar à tabela `imovel` uma nova coluna chamada `nome_imovel`, do tipo texto com tamanho máximo de 100 caracteres. Essa coluna deve servir para identificar cada imóvel de forma textual.

### Passo 10 - Inserção de Dados na Tabela Imovel
Insira pelo menos **10 registros** na tabela `imovel`, utilizando dados consistentes e coerentes com o contexto da corretora de imóveis.

### Passo 11 - Criação da Tabela Venda
Crie a tabela `venda` no banco de dados `corretora`, seguindo a estrutura e as especificações do diagrama lógico da corretora de imóveis. Certifique-se de definir corretamente os campos, tipos de dados e restrições de integridade.

### Passo 12 - Inserção de Dados na Tabela Venda
Insira no mínimo **5 registros** na tabela `venda`, com dados reais e coerentes que representem as transações de venda realizadas pela corretora.

### Passo 13 - Consulta Relacional das Vendas
Crie uma consulta SQL que retorne as seguintes informações de todas as vendas:  
- Nome do comprador  
- Nome do proprietário do imóvel  
- Nome do corretor responsável pela venda  

A consulta deve utilizar relacionamentos (joins) entre as tabelas relacionadas.

### Passo 14 - Criação de uma View de Relatório
Com base na consulta criada no passo anterior, crie uma **view** que encapsule a lógica da consulta, permitindo sua reutilização para exibição de dados de vendas da corretora.

### Passo 15 - Criação de um Usuário Visualizador
Crie um usuário chamado `visualizador` com uma senha segura, garantindo que esse usuário tenha **apenas permissão de leitura** sobre a view criada no passo anterior.

### Passo 16 - Entrega das Credenciais para Validação
Envie via Google Sala de Aula as credenciais do servidor PostgreSQL criado no Azure, incluindo:  
- Host  
- Database  
- User (deve ser o usuário criado com permissão restrita)  
- Password  
- Port  

Essas informações serão utilizadas para validação da entrega, garantindo que o usuário possui acesso restrito conforme solicitado.

---


