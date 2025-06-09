## 🔐 1. Princípios de Identidade no Azure

### Azure Active Directory (Azure AD)
- Serviço de gerenciamento de identidades baseado na nuvem da Microsoft.
- Permite autenticação e autorização de usuários, dispositivos e aplicativos.
- Integração com serviços da Microsoft (como Office 365) e aplicativos de terceiros.
- **Funções principais**:
  - Autenticação: Verifica a identidade do usuário.
  - Autorização: Garante acesso somente ao que for permitido.

### Tipos de Identidade
- **Conta de usuário**: Individual, vinculada a um colaborador.
- **Conta de serviço**: Usada por aplicativos ou serviços para se autenticar.
- **Identidade externa (B2B)**: Usuários convidados de fora da organização.

## 🔑 2. Controle de Acesso no Azure

### RBAC (Role-Based Access Control)
- Permite o controle de quem pode realizar ações em recursos do Azure.
- Baseado em três componentes:
  - **Security Principal** (usuário, grupo, app)
  - **Role Definition** (ex: Leitor, Colaborador, Proprietário)
  - **Scope** (nível de aplicação: grupo de recursos, assinatura, recurso)

### Políticas do Azure
- Usadas para **forçar regras** e padrões em recursos.
- Exemplo: impedir a criação de VMs fora da região específica.

### Azure Blueprints
- Ferramenta para orquestrar políticas, RBAC e recursos em conjunto.
- Útil para configurar ambientes consistentes e em conformidade.

## 🛡️ 3. Segurança no Azure

### Segurança de Rede
- **NSG (Network Security Group)**: Filtra tráfego para recursos em uma VNet.
- **Azure Firewall**: Firewall gerenciado com regras de aplicação e rede.
- **Azure DDoS Protection**: Proteção contra ataques de negação de serviço.

### Segurança de Dados
- **Criptografia em repouso**: Usando Azure Storage Service Encryption.
- **Criptografia em trânsito**: TLS/SSL para comunicação segura.
- **Azure Key Vault**: Gerencia chaves, segredos e certificados com segurança.

### Serviços de Segurança
- **Microsoft Defender for Cloud**:
  - Avaliação contínua de segurança.
  - Recomendações de correção.
- **Microsoft Sentinel**:
  - SIEM baseado em nuvem.
  - Coleta e análise de logs de segurança.
- **Azure Security Center** (agora parte do Defender for Cloud):
  - Monitoramento e resposta a ameaças.

## 🔐 4. Conformidade e Gerenciamento de Identidade

### MFA (Autenticação Multifator)
- Adiciona uma camada extra de segurança (ex: senha + aplicativo de autenticação).
- Reduz riscos de acesso não autorizado.

### Conditional Access
- Políticas que aplicam condições para acesso, como:
  - Localização.
  - Dispositivo.
  - Estado de risco da sessão.

### Compliance
- Azure oferece mais de 90 certificações de conformidade.
- Ferramentas como **Compliance Manager** e **Service Trust Portal** ajudam a verificar e gerenciar requisitos regulatórios.
