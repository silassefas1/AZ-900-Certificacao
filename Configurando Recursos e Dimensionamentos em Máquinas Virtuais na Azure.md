# 📘 Guia Rápido: Criação de VMs e Redes no Microsoft Azure

Este documento fornece um resumo dos passos necessários para criar máquinas virtuais (VMs) e configurar redes no ambiente Azure, utilizando o portal web ou a linha de comando (Azure CLI).

---

## 🏗️ Pré-requisitos

- Conta ativa no Azure
- Grupo de recursos criado (Resource Group)
- Permissões de Contributor ou superiores

---

## 🌐 1. Criação de Rede Virtual (VNet)

### Via Portal

1. Acesse **Rede Virtual** no Azure Portal.
2. Clique em **Criar**.
3. Defina:
   - Nome da VNet
   - Espaço de endereçamento (ex: `10.0.0.0/16`)
   - Sub-rede padrão (ex: `10.0.1.0/24`)
   - Região
4. Clique em **Revisar + Criar** e depois **Criar**.


## 🖥️ 2. Criação da Máquina Virtual (VM)

### Via Portal

1. Acesse **Máquinas Virtuais** e clique em **Criar**.
2. Configure:
   - Nome da VM
   - Região e grupo de recursos
   - Imagem (ex: Ubuntu, Windows Server)
   - Tamanho da VM
   - Usuário e senha/SSH
   - Rede virtual (selecione a criada anteriormente)
3. Defina regras de firewall (ex: permitir SSH ou RDP).
4. Clique em **Revisar + Criar** e depois **Criar**.


## ✅ Conclusão

Após seguir esses passos, você terá uma VM funcional dentro de uma rede virtual no Azure, pronta para testes, desenvolvimento ou produção.


