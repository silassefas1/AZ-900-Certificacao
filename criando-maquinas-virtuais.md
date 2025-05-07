# 🚀 Criação e Configuração de Máquina Virtual no Microsoft Azure

Este documento resume o processo de criação e configuração de uma Máquina Virtual (VM) no Microsoft Azure, utilizando o portal web.

---

## ✅ O que é necessário

* Conta ativa no Azure com permissões para criação de recursos
* Grupo de recursos (novo ou existente)
* Escolha do sistema operacional, tamanho da VM e região

---

## 🛠️ Etapas Principais

* **Acesso ao portal Azure**: Entrar em [https://portal.azure.com](https://portal.azure.com)
* **Criação da VM**: Navegar até **“Máquinas Virtuais”** e iniciar uma nova instância
* **Configuração básica**: Definir nome, imagem do SO, região, autenticação (senha ou chave SSH) e tamanho da VM
* **Discos e rede**: Escolher o tipo de disco (HDD/SSD) e configurar a rede virtual e as regras de acesso (NSG)
* **Revisão e criação**: Validar as configurações e clicar em **"Criar"**
* **Conexão**: Após provisionamento, conectar via **SSH (Linux)** ou **RDP (Windows)**

---

## ⚠️ Dica Importante

Para evitar **cobranças indevidas**, lembre-se de **excluir a VM e o grupo de recursos** caso não sejam mais necessários.

---

## 📝 Observações sobre SLA e Disponibilidade

1. O **SLA de disponibilidade** não se aplica diretamente a VMs individuais. Ele depende da configuração e modelo de alta disponibilidade escolhido pelo usuário.
2. A **disponibilidade** da VM está vinculada às **zonas de disponibilidade** selecionadas. É possível configurar até 3 zonas, com replicação dos dados entre elas.
3. O uso de múltiplas zonas pode gerar custos adicionais, mas em contrapartida, também reduz o tempo de indisponibilidade ao aumentar a resiliência da aplicação.

---

# 📊 Tabela de SLA

| SLA     | Tempo de inatividade por semana | Tempo de inatividade por mês | Tempo de inatividade por ano |
| ------- | ------------------------------- | ---------------------------- | ---------------------------- |
| 99%     | 1,68 hora                       | 7,2 horas                    | 3,65 dias                    |
| 99,9%   | 10,1 minutos                    | 43,2 minutos                 | 8,76 horas                   |
| 99,95%  | 5 minutos                       | 21,6 minutos                 | 4,38 horas                   |
| 99,99%  | 1,01 minuto                     | 4,32 minutos                 | 52,56 minutos                |
| 99,999% | 6 segundos                      | 25,9 segundos                | 5,26 minutos                 |

🔗 [Visualizar tabela oficial de SLA da Microsoft](https://learn.microsoft.com/en-us/power-platform/well-architected/reliability/metrics)
