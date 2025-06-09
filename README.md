# criandomaqvirtualnoazure

# Criando Máquinas Virtuais no Microsoft Azure

Este guia explica como criar e gerenciar Máquinas Virtuais (VMs) no Microsoft Azure.

## Pré-requisitos
- Conta ativa no Azure ([crie uma gratuitamente](https://azure.microsoft.com/free/))
- Acesso ao [Portal Azure](https://portal.azure.com)
- Permissões para criar recursos na assinatura

## Passo a Passo para Criação de VM

### 1. Acessar o Portal Azure
1. Faça login no [Portal Azure](https://portal.azure.com)
2. Clique em "Criar um recurso" no menu esquerdo

### 2. Selecionar Máquina Virtual
1. Na página "Novo", selecione "Computação"
2. Escolha "Máquina Virtual"

### 3. Configurar Básicos
Preencha as informações básicas:
- **Assinatura**: Selecione sua assinatura
- **Grupo de recursos**: Crie um novo ou selecione existente
- **Nome da máquina virtual**: (ex: vm-demo-01)
- **Região**: Selecione a mais próxima de você
- **Imagem**: Escolha entre Windows Server ou Linux (Ubuntu, CentOS, etc.)
- **Tamanho**: Selecione conforme necessidade (B1s para testes)

### 4. Configurar Credenciais
- Para Windows:
  - Nome de usuário
  - Senha (mínimo 12 caracteres)
- Para Linux:
  - Nome de usuário
  - Chave SSH ou senha

### 5. Configurar Regras de Entrada
Na aba "Rede":
- Selecione ou crie uma rede virtual
- Configure o Grupo de Segurança de Rede (NSG)
- Habilite portas conforme necessidade (ex: RDP 3389 para Windows, SSH 22 para Linux)

### 6. Revisar e Criar
1. Revise todas as configurações
2. Clique em "Criar" para iniciar a implantação

## Conectando à VM

### Windows (via RDP)
1. Após a implantação, vá até o recurso da VM
2. Clique em "Conectar" > "RDP"
3. Baixe o arquivo RDP e execute

### Linux (via SSH)
1. Acesse o recurso da VM
2. Clique em "Conectar" > "SSH"
3. Use o comando fornecido no terminal

## Gerenciamento Básico
- **Iniciar/Parar**: Controles na página de visão geral
- **Redimensionar**: Opção "Tamanho" no menu
- **Monitoramento**: Métricas disponíveis na seção "Monitoramento"

## Boas Práticas
✔️ Sempre pare VMs não utilizadas para economizar custos  
✔️ Use discos gerenciados para melhor confiabilidade  
✔️ Configure backups regulares  
✔️ Aplique tags para organização  

## Limpeza de Recursos
Para evitar cobranças indesejadas:
1. Vá para o Grupo de Recursos
2. Selecione "Excluir grupo de recursos"
3. Confirme o nome e clique em "Excluir"

## Suporte e Ajuda
- [Documentação Oficial Azure VMs](https://docs.microsoft.com/azure/virtual-machines/)
- [Fórum de Suporte Azure](https://azure.microsoft.com/support/forums/)
- [Calculadora de Custos Azure](https://azure.microsoft.com/pricing/calculator/)
