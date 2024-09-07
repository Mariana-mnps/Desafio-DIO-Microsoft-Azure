## Criar e Configurar Máquinas Virtuais no Azure

### Passo 1: Acessar o Portal Azure

   - Abra o navegador e vá para portal azure.
  
### Passo 2: Criar uma Nova Máquina Virtual

   - No menu à esquerda, clique em **“Criar um recurso”**.
   - Na barra de pesquisa, digite “Máquina Virtual” e selecione **“Máquina Virtual”** nos resultados.
   - Clique em **“Criar”**.

3. **Preencher os Detalhes**:
   - **Assinatura**: Escolha a assinatura do Azure que será usada.
   - **Grupo de Recursos**: Selecione um grupo de recursos existente ou crie um novo.
   - **Nome da Máquina Virtual**: Insira um nome exclusivo para sua VM.
   - **Região**: Escolha a região onde a VM será criada. (Regiões mais próximas aos usuários oferece melhor performance)
   - **Imagem**: Selecione o sistema operacional da VM (por exemplo, Ubuntu, Windows Server).
   - **Tamanho**: Clique em **“Selecionar tamanho”** para escolher a configuração de hardware (CPU, memória) adequada às suas necessidades. Após escolher, clique em **“Selecionar”**. 
     - **Importante**: manter a opção de "excluir com VM" selecionada
   - **Nome de Usuário e Senha**: Configure um nome de usuário e uma senha para acessar a VM. Você também pode usar uma chave SSH para autenticação se preferir.

4. **Configurar Disco**:
   - **Tipo de Disco**: Escolha entre SSD (Standard SSD, Premium SSD) ou HDD (Standard HDD).
   - **Disco do Sistema Operacional**: Configure o disco do sistema operacional de acordo com suas necessidades.

5. **Configurar Rede**:
   - **Rede Virtual**: Selecione uma rede virtual existente ou crie uma nova.
   - **Sub-rede**: Escolha uma sub-rede dentro da rede virtual.
   - **IP Público**: Defina se a VM deve ter um IP público.
   - **Grupo de Segurança de Rede (NSG)**: Configure as regras de firewall para permitir o tráfego necessário (por exemplo, portas 22 para SSH ou 3389 para RDP).

6. **Configurações Adicionais**:
   - **Extensões**: Adicione extensões se precisar (por exemplo, para instalação de software adicional).
   - **Backup**: Configure opções de backup, se desejado.
   - **Monitoramento**: Habilite o monitoramento se quiser coletar métricas e logs.

7. **Revisar e Criar**:
   - Revise todas as configurações.
   - Clique em **“Criar”** para iniciar a criação da VM.

### Passo 3: Configurar a Máquina Virtual Após a Criação

   - No menu à esquerda, clique em **“Máquinas Virtuais”**.
   - Selecione a VM que você criou.

2. **Configurar Recursos e Dimensionamento**:
   - **Dimensionamento**:
     - No painel da VM, clique em **“Tamanho”** no menu à esquerda.
     - Escolha um novo tamanho de VM se você precisar ajustar os recursos (CPU, memória). Clique em **“Selecionar”** para aplicar a mudança.

   - **Configurações de Disco**:
     - Para adicionar discos adicionais, vá até **“Discos”** no menu da VM e clique em **“+ Adicionar disco”**. Configure o disco e clique em **“Salvar”**.

   - **Configurações de Rede**:
     - Para alterar configurações de rede, clique em **“Rede”** no menu da VM. Aqui você pode alterar a rede virtual, sub-rede ou configurações de IP.

   - **Configurações de Backup e Monitoramento**:
     - Se você deseja configurar ou ajustar o backup, vá até **“Backup”** e configure conforme necessário.
     - Para ajustes no monitoramento, clique em **“Insights”** e ajuste as configurações de coleta de métricas e logs.

### Passo 4: Acessar e Gerenciar a Máquina Virtual

1. **Conectar à Máquina Virtual**:
   - Para máquinas virtuais Windows:
     - Clique em **“Conectar”** e selecione **“RDP”**. Baixe o arquivo RDP e use-o para se conectar via Remote Desktop.
   - Para máquinas virtuais Linux:
     - Clique em **“Conectar”** e selecione **“SSH”**. Use o comando SSH fornecido no terminal para conectar à VM.

2. **Gerenciar a Máquina Virtual**:
   - No painel da VM, você pode **reiniciar**, **desligar** ou **encerrar** a máquina virtual conforme necessário.

3. **Configurar Alertas e Diagnósticos**:
   - Para configurar alertas, vá para **“Alertas”** e defina regras para monitorar o estado e o desempenho da VM.
   - Para diagnósticos avançados, clique em **“Diagnóstico e solução de problemas”** e configure ferramentas como logs e métricas adicionais.

### Passo 5: Monitorar e Manter a Máquina Virtual

1. **Monitorar Desempenho**:
   - No painel da VM, clique em **“Monitoramento”** para visualizar gráficos de uso de CPU, memória, e outros recursos.

2. **Atualizar e Manter**:
   - Mantenha a VM atualizada com patches e atualizações de segurança.
   - Realize backups regulares e verifique a integridade dos dados.

3. **Gerenciar Custos**:
   - Monitore o uso e os custos da VM através da seção **“Custos e Faturamento”** no portal do Azure.

---
