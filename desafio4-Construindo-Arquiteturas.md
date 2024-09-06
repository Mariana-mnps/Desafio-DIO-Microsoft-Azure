# Construindo Arquiteturas no Azure

### Passo 1: Criar um Grupo de Recursos
- Um Grupo de Recursos é um container que agrupa recursos relacionados e facilita o gerenciamento, controle e monitoramento.

 #### Acessar o Portal Azure:

- Vá para portal.azure.com e faça login com suas credenciais.
  
 #### Criar um Novo Grupo de Recursos:

- No painel esquerdo, clique em “Grupos de recursos”.
- Clique em “+ Adicionar” ou “Criar grupo de recursos”.
  
 #### Preencher os Detalhes do Grupo de Recursos:

- Nome do Grupo de Recursos: Insira um nome exclusivo para o grupo de recursos.
- Assinatura: Selecione a assinatura do Azure onde o grupo de recursos será criado.
- Localização: Escolha a região onde você deseja armazenar os metadados do grupo de recursos. Isso não afeta a localização dos recursos em si.

 #### Criar o Grupo de Recursos:

- Clique em “Revisar + criar” para revisar as configurações.
- Clique em “Criar” para criar o grupo de recursos.
  
### Passo 2: Criar uma Rede Virtual
Uma Rede Virtual (VNet) fornece isolamento e conectividade para suas máquinas virtuais e outros recursos na nuvem.

#### Criar uma Nova Rede Virtual:

- No painel esquerdo, clique em “Redes virtuais”.
- Clique em “+ Adicionar” ou “Criar”.
  
#### Preencher os Detalhes da Rede Virtual:

- Nome: Insira um nome exclusivo para a rede virtual.
- Grupo de Recursos: Selecione o grupo de recursos que você criou anteriormente.
- Localização: Escolha a região onde a rede virtual será criada.

#### Configurar as Configurações de IP:

- Espaço de Endereços IP: Insira o intervalo de endereços IP em formato CIDR (por exemplo, 10.0.0.0/16).
- Sub-redes: Clique em “Adicionar uma sub-rede” para definir uma sub-rede. Preencha o nome da sub-rede e o intervalo de endereços IP para a sub-rede (por exemplo, 10.0.1.0/24).

#### Configurações Adicionais (opcional):

Configure recursos adicionais como gateways VPN ou conectividade ExpressRoute se necessário.

#### Criar a Rede Virtual:

- Clique em “Revisar + criar” para revisar as configurações.
- Clique em “Criar” para criar a rede virtual.

### Passo 3: Criar Regras de Segurança (Grupo de Segurança de Rede)
Grupos de Segurança de Rede (NSGs) são usados para controlar o tráfego de entrada e saída para e de suas instâncias de recursos.

#### Criar um Novo Grupo de Segurança de Rede:

- No painel esquerdo, clique em “Grupos de segurança de rede”.
- Clique em “+ Adicionar” ou “Criar grupo de segurança de rede”.

#### Preencher os Detalhes do NSG:

- Nome: Insira um nome exclusivo para o grupo de segurança de rede.
- Grupo de Recursos: Selecione o grupo de recursos onde o NSG será criado.
- Localização: Escolha a região onde o NSG será criado.

#### Configurar Regras de Segurança:

Após a criação, você pode adicionar regras de segurança para controlar o tráfego:

- Regras de Entrada: Clique em “Regras de entrada” e, em seguida, em “+ Adicionar” para criar uma nova regra. Preencha os seguintes campos:
- Nome: Nome da regra.
- Prioridade: A prioridade da regra (um número menor tem prioridade mais alta).
- Origem: Selecione a origem do tráfego (por exemplo, "Qualquer" ou um IP específico).
- Porta de Destino: Especifique a porta ou intervalo de portas (por exemplo, 80 para HTTP).
- Ação: Selecione “Permitir” ou “Negar”.
- Protocolos: Selecione TCP, UDP ou qualquer.
- Regras de Saída: Configure regras semelhantes para o tráfego de saída.

#### Associar o NSG à Rede Virtual ou Sub-rede:

- No painel do NSG, vá para “Sub-redes” e clique em “+ Associe”.
- Selecione a rede virtual e a sub-rede à qual você deseja aplicar o NSG.

#### Revisar e Concluir:

- Após configurar todas as regras e associações, revise as configurações.
- Clique em “Revisar + criar” e depois em “Criar” para concluir a criação do NSG.
