## **Gerenciando Políticas de Acesso no Azure**

### **Passo 1: Acessar o Portal do Azure**

1. **Entrar no Portal do Azure**
   - Acesse portal.azure.com e faça login com suas credenciais de administrador.

### **Passo 2: Gerenciar Acessos com Azure Role-Based Access Control (RBAC)**

#### **2.1. Atribuir Funções a Usuários, Grupos ou Entidades de Serviço**

1. **Acessar o Recurso Desejado**
   - Navegue até o recurso específico para o qual deseja gerenciar o acesso (por exemplo, uma máquina virtual, um banco de dados, um grupo de recursos).

2. **Abrir Controle de Acesso (IAM)**
   - No menu à esquerda, selecione **“Controle de Acesso (IAM)”**.

3. **Adicionar Atribuição de Função**
   - Clique em **“+ Adicionar”** e selecione **“Atribuição de função”**.
   - Escolha a função apropriada (por exemplo, Leitor, Contribuidor, Proprietário) que define o nível de acesso.
   - Selecione o usuário, grupo ou entidade de serviço ao qual deseja atribuir a função.
   - Defina o escopo da atribuição (nível de assinatura, grupo de recursos ou recurso específico) e clique em **“Salvar”**.

#### **2.2. Revisar e Gerenciar Atribuições de Função**

1. **Visualizar Atribuições de Função**
   - No painel **“Controle de Acesso (IAM)”**, clique em **“Atribuições de função”** para visualizar todas as atribuições de função atuais para o recurso.

2. **Modificar ou Remover Atribuições**
   - Selecione uma atribuição de função existente para editar ou remover.
   - Para editar, clique em **“Editar”** e ajuste a função ou o escopo conforme necessário.
   - Para remover, clique em **“Excluir”** e confirme a ação.

### **Passo 3: Gerenciar Políticas de Acesso Condicional com Azure AD**

#### **3.1. Criar Políticas de Acesso Condicional**

1. **Acessar Acesso Condicional**
   - No Azure Active Directory, selecione **“Segurança”** e depois **“Políticas de Acesso Condicional”**.

2. **Criar Nova Política**
   - Clique em **“+ Nova política”**.
   - Defina um nome para a política e configure as condições, como aplicativos em nuvem, usuários e grupos, localizações e dispositivos.
   - Configure as ações, como exigir Multi-Factor Authentication (MFA) ou bloquear o acesso.
   - Clique em **“Criar”** para aplicar a política.

#### **3.2. Monitorar e Ajustar Políticas de Acesso Condicional**

1. **Revisar Relatórios de Acesso Condicional**
   - No painel de **“Políticas de Acesso Condicional”**, selecione **“Relatórios”** para revisar o impacto das políticas.
   - Analise as métricas e eventos para entender como as políticas estão sendo aplicadas e se há necessidades de ajustes.

2. **Ajustar Políticas**
   - Com base nos relatórios e feedback, ajuste suas políticas para melhorar a segurança e o acesso conforme necessário.

### **Passo 4: Gerenciar Políticas de Governança com Azure Policy**

#### **4.1. Criar e Aplicar Políticas**

1. **Acessar Azure Policy**
   - No portal do Azure, selecione **“Política”** no menu à esquerda.

2. **Criar Nova Política**
   - Clique em **“+ Criar política”**.
   - Preencha os detalhes da política, como nome, descrição e definição.
   - Configure as regras da política para definir quais recursos devem estar conformes e as ações a serem tomadas em caso de não conformidade.
   - Clique em **“Criar”** para criar a política.

3. **Associar Política a um Escopo**
   - Após criar a política, vá para **“Associações”**.
   - Clique em **“+ Associar”** e selecione o escopo desejado (assinatura, grupo de recursos, etc.).
   - Defina as configurações de exclusão e outras opções conforme necessário e clique em **“Criar”**.

#### **4.2. Monitorar e Auditar Políticas**

1. **Verificar Conformidade**
   - No painel **“Política”**, vá para **“Conformidade”** para verificar o status das políticas aplicadas.
   - Revise os recursos que estão em conformidade e aqueles que não estão, e tome as ações necessárias para corrigir as não conformidades.

2. **Visualizar Logs e Relatórios**
   - No portal do Azure, acesse **“Monitoramento”** e selecione **“Logs”** para visualizar logs detalhados sobre a aplicação de políticas e ações.

### **Passo 5: Revisar e Atualizar Acessos e Políticas Regularmente**

1. **Revisar Permissões e Políticas**
   - Realize revisões periódicas das permissões de acesso e das políticas de governança para garantir que ainda estejam alinhadas com as necessidades e requisitos da organização.

2. **Atualizar Políticas e Funções**
   - Atualize as políticas e funções conforme necessário para refletir mudanças na infraestrutura, requisitos de negócios ou regulamentações.
