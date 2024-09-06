# Configuração de uma Instância de Banco de Dados no Azure

### Passo 1: Acessar o Portal Azure
- Acesse o Portal Azure: Abra o seu navegador e vá para portal.azure.com. Faça login com suas credenciais.
  
### Passo 2: Criar um Novo Banco de Dados
- Clique em “Criar um recurso”: No painel do portal, clique no botão “Criar um recurso” no menu à esquerda.
- Escolha “Banco de Dados SQL”: Na barra de pesquisa, digite “Banco de Dados SQL” e selecione “Banco de Dados SQL” na lista de resultados. Em seguida, clique em “Criar”.

### Passo 3: Configurar o Banco de Dados SQL
#### Configurações Básicas:

- Assinatura: Escolha a assinatura do Azure que será usada.
- Grupo de Recursos: Selecione um grupo de recursos existente ou crie um novo.
- Nome do Banco de Dados: Digite um nome para seu banco de dados.
- Servidor: Selecione um servidor existente ou crie um novo. Para criar um novo servidor:
- Nome do Servidor: Forneça um nome único para o servidor.
- Localização: Escolha a região onde o servidor será criado.
- Nome de Usuário do Administrador: Defina um nome de usuário para o administrador do banco de dados.
- Senha do Administrador: Defina uma senha segura.

### Configurações de Desempenho:

- Modelo de Compra: Escolha entre "Baseado em DTU" ou "Baseado em vCore" (o modelo baseado em vCore é recomendado para maior flexibilidade e controle).
- Camada de Serviço: Escolha a camada de serviço (por exemplo, Básico, Standard, Premium ou General Purpose, Business Critical).
- Configurações de Capacidade: Ajuste a capacidade de acordo com suas necessidades.

#### Configurações Adicionais:

- Backup e Recuperação: Configure as opções de backup conforme necessário.
- Segurança: Configure opções adicionais de segurança, como a criptografia.
  
### Criar:

- Revise todas as configurações e clique em “Criar” para iniciar o processo de criação do banco de dados.
  
### Passo 4: Configurar o Acesso

- Configurar Regras de Firewall: Após a criação, configure as regras de firewall para permitir acesso ao banco de dados a partir de seu IP ou faixa de IPs.
- Navegue até o servidor SQL criado, selecione "Regras de firewall e virtual networks" e adicione uma nova regra de firewall.

### Passo 5: Conectar ao Banco de Dados
- Obter a String de Conexão: No portal, navegue até o banco de dados SQL e selecione "Visão geral" para obter a string de conexão.
- Conectar com uma Ferramenta: Use uma ferramenta como SQL Server Management Studio (SSMS) ou Azure Data Studio para se conectar ao banco de dados usando a string de conexão.
