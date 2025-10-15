# Dashboard corporativo com integração com MySQL e Azure

# Objetivo

Criar um sistema completo de banco de dados Company no Azure SQL Server e integrá-lo ao Power BI para visualização de dados e geração de relatórios.

## Pré-requisitos

 Antes de começar, certifique-se de ter:

* Conta ativa no Azure com permissão para criar recursos.

* Power BI Desktop instalado.

* Conhecimentos básicos de SQL.

* Navegador moderno.

# Passo a Passo
# 1. Criar o Banco de Dados no Azure SQL Server

  1 - Acesse o portal do Azure: https://portal.azure.com

  2 - Clique em Criar um recurso → Banco de Dados SQL.

  3 - Preencha as informações:

    Grupo de Recursos: CompanyResources (crie um novo, se necessário)

    Nome do Servidor SQL: companyserverxyz

    Banco de Dados: Company

    Versão do SQL: Última disponível

    Preço/Performance: Selecione conforme necessidade (Ex.: Basic para teste)

  4 - Clique em Revisar + criar → Criar.

  5 -Aguarde a implantação do servidor e do banco de dados.

# 2. Configurar Acesso ao Banco de Dados

  1 - No Azure, acesse o Servidor SQL criado.

  2 - Clique em Configurações de Firewall.

  3 -Adicione seu IP para permitir conexão externa.

  4 - Anote o nome do servidor, usuário e senha — você precisará para conectar no Power BI.

# 3. Criar Tabelas e Estrutura do Banco

  1 - Abra o Query Editor no Azure SQL Server ou use SQL Server Management Studio (SSMS).

  2 - Execute comandos SQL para criar tabelas do sistema Company.
  
  3 -Popule as tabelas com dados

# 4. Conectar Power BI ao Azure SQL

  1 - Abra Power BI Desktop.

  2 - Clique em Obter Dados → Banco de Dados SQL Server.

  3 - Insira:

    Servidor: companyserverxyz.database.windows.net

    Banco de dados: Company

  4 - Selecione Autenticação do SQL e informe usuário/senha.

  5 - Clique em Conectar e selecione as tabelas desejadas.

5. Criar Relatórios no Power BI

  1 - No Power BI, adicione visualizações como tabelas, gráficos de barras e gráficos de pizza.

  2 - Use campos do banco para gerar métricas:

    Total de funcionários por departamento

    Média de tempo de contratação

    Crescimento de equipe por período

  3 - Configure filtros e slicers para interação com os dados.

6. Publicar Relatórios no Power BI Service

  1 - Clique em Publicar → selecione seu workspace no Power BI Service.

  2 - Configure agendamento de atualização de dados para manter os relatórios sincronizados com o Azure SQL.
