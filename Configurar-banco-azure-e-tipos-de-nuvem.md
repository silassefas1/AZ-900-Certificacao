# Resumo: Configuração de Instância de Banco de Dados na Microsoft Azure

## O que é o Azure?

O **Microsoft Azure** é uma plataforma de computação em nuvem que oferece uma variedade de serviços, incluindo hospedagem e gerenciamento de bancos de dados relacionais e não relacionais.

## Passos para Criar uma Instância de Banco de Dados no Azure

1. **Acessar o Portal Azure**
   - https://portal.azure.com
   - Requer uma conta Microsoft com assinatura ativa (pode ser gratuita).

2. **Criar um Recurso de Banco de Dados**
   - No menu "Criar um recurso", buscar por "SQL Database" ou outro tipo (MySQL, PostgreSQL, etc.).
   - Selecionar o tipo de banco desejado (por exemplo, **Azure SQL Database**).

3. **Configurar a Instância**
   - **Nome do banco de dados**
   - **Servidor lógico** (criar um novo ou usar existente)
   - **Localização (região)** do data center
   - **Camada de preço** (Free, Basic, Standard, Premium)

4. **Criar um Servidor Lógico**
   - Definir nome, login de administrador e senha
   - Escolher a região

5. **Regras de Firewall**
   - Adicionar IPs confiáveis que poderão acessar o banco
   - Permitir acesso ao Azure (opcional)

6. **Revisar e Criar**
   - Verificar configurações
   - Clicar em "Criar"

7. **Conectar ao Banco**
   - Usar ferramentas como **Azure Data Studio**, **SQL Server Management Studio (SSMS)** ou aplicativos customizados.
   - Conectar-se usando os dados do servidor (host, login e senha).

## Dicas Importantes

- **Use a camada gratuita** para testes e aprendizado.
- **Nunca compartilhe credenciais** do banco em repositórios públicos.
- **Monitore a performance** via painel do Azure.
- Faça **backup regular** das suas bases de dados.
- **Feche instâncias não utilizadas** para evitar cobranças.

## Modelos de Tipos de Nuvem ☁️

### IaaS (Infrastructure as a Service)
> **Exemplo**: Azure Virtual Machines  
Você gerencia: SO, aplicativos, runtime, dados.  
Azure gerencia: infraestrutura, rede, armazenamento.

###  PaaS (Platform as a Service)
> **Exemplo**: Azure SQL Database  
Você gerencia: dados e aplicativos.  
Azure gerencia: SO, runtime, middleware, infraestrutura.

###  SaaS (Software as a Service)
> **Exemplo**: Microsoft 365, Outlook  
Você apenas **usa o serviço final**.  
Azure gerencia tudo por trás dos panos.

### Comparação:

| Modelo | Você gerencia | Provedor gerencia |
|--------|----------------|-------------------|
| IaaS   | App, Dados, SO | Hardware, rede    |
| PaaS   | App, Dados     | SO, infraestrutura |
| SaaS   | Uso do app     | Tudo               |

---

## Modelo de Responsabilidade Compartilhada 

O modelo de responsabilidade compartilhada define **quem cuida de quê** entre o **usuário** e o **provedor de nuvem (Azure)**.

### Exemplo de Divisão:

| Área                          | Responsável |
|-------------------------------|-------------|
| Infraestrutura física         | Azure       |
| Hospedagem e rede             | Azure       |
| Segurança física              | Azure       |
| Controle de acesso (usuário)  | Cliente     |
| Gerenciamento de identidade   | Cliente     |
| Dados, senhas e permissões    | Cliente     |

**Resumo**: A **segurança da nuvem** é responsabilidade da Azure. A **segurança na nuvem** (senhas, dados, acessos) é responsabilidade do cliente.


