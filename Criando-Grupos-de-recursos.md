# Criando Grupos de Recursos e uma VNet no Azure

## O que são Grupos de Recursos e VNet?

- **Grupo de Recursos**: É uma unidade lógica que agrupa recursos do Azure, como máquinas virtuais, redes, bancos de dados, etc. Ele facilita o gerenciamento, monitoramento e controle de acesso dos recursos agrupados.

- **VNet (Virtual Network)**: É a rede virtual do Azure, equivalente a uma rede local tradicional, mas na nuvem. Ela permite a comunicação entre recursos do Azure, com a internet e com redes locais, de forma segura.

---

## 🛠️ Passo a Passo para Criar um Grupo de Recursos e uma VNet

### Pré-requisitos:
- Conta no [Microsoft Azure](https://portal.azure.com/)
- Permissões suficientes para criar recursos (ex: proprietário ou colaborador)

---

### 1️⃣ Criar um Grupo de Recursos

#### Via Portal Azure:
1. Acesse o [portal Azure](https://portal.azure.com/)
2. No menu lateral, clique em **"Grupos de recursos"**
3. Clique em **"+ Criar"**
4. Escolha a **assinatura** e **região** 
5. Dê um **nome** para o grupo 
6. Clique em **"Revisar + Criar"** e depois **"Criar"**

---

### 2️⃣ Criar uma VNet (Virtual Network)

#### Via Portal Azure:
1. Acesse o menu "Redes virtuais"
2. Clique em **"+ Criar"**
3. Selecione o **grupo de recursos** criado anteriormente
4. Dê um **nome** para a VNet
5. Escolha a **região** (deve ser a mesma do grupo)
6. Configure o **espaço de endereços** 
7. Clique em **"Revisar + Criar"** e depois **"Criar"**

---
