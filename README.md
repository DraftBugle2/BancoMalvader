
# Banco Malvader

## Descrição do Projeto

O Banco Malvader é um sistema desenvolvido para gerenciar contas bancárias, transações e operações financeiras em um ambiente seguro e intuitivo. Este repositório contém o código-fonte, diagramas e scripts necessários para executar e entender o projeto.

---

## Estrutura do Projeto

- **`controllers`**: Gerencia a lógica central da aplicação, conectando modelos e visualizações.
- **`dao`**: Contém funções para acesso e manipulação do banco de dados.
- **`models`**: Define as classes e estruturas que representam as entidades do sistema, como contas, clientes e transações.
- **`startpoint`**: Ponto inicial para execução da aplicação.
- **`utils`**: Inclui funções auxiliares, como validações e configurações.
- **`view`**: Contém elementos de interface para interação com os usuários.

---

## Configuração do Banco de Dados

O arquivo `banco_malvader_db.sql` contém o script necessário para criar e configurar o banco de dados. Certifique-se de executar este script em seu ambiente SQL antes de iniciar a aplicação.

---

## Pré-requisitos

- Java JDK (versão 22 ou superior)
- Ambiente de desenvolvimento integrado (IDE) configurado para projetos Java
- Banco de dados SQL compatível

---

## Executando o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/DraftBugle2/BancoMalvader.git
   ```
2. Configure o banco de dados executando o script `banco_malvader_db.sql`.
3. Importe o projeto em sua IDE.
4. Execute o ponto de entrada principal localizado em `startpoint`.

---

## Diagramas

Os diagramas do sistema estão localizados no diretório `diagramas`. Eles fornecem uma visão detalhada da arquitetura e do fluxo do sistema.

## Descrição Detalhada das Pastas

### **`controllers`**
Gerencia a lógica central da aplicação, conectando modelos e visualizações:
- **`BancoController.java`**: Controla operações relacionadas ao banco, como gerenciamento de contas e transações.
- **`UsuarioController.java`**: Gerencia ações relacionadas aos usuários, incluindo autenticação e permissões.

---

### **`dao`**
Responsável pelo acesso a dados e interação com o banco de dados:
- **`BancoDAO.java`**: Contém métodos para acessar e manipular informações sobre bancos.
- **`ClienteDAO.java`**: Gerencia a persistência de dados dos clientes.
- **`ConnectionFactory.java`**: Configura e fornece conexões com o banco de dados.
- **`FuncionarioDAO.java`**: Realiza operações relacionadas aos funcionários no banco de dados.

---

### **`models`**
Define as classes que representam as entidades do sistema:
- **`Cliente.java`**: Modelo para representar os clientes do banco.
- **`Conta.java`**: Representa contas bancárias com atributos como saldo e número da conta.
- **`Endereco.java`**: Define o modelo para informações de endereço de clientes ou funcionários.
- **`Transacao.java`**: Modelo para representar transações bancárias.

---

### **`startpoint`**
Ponto inicial e arquivos auxiliares para iniciar a aplicação:
- **`BancoMalvader.java`**: Classe principal que inicia a aplicação.
- **`ConexaoBanco.java`**: Gerencia a conexão inicial com o banco de dados.
- **`Relatorio.java`**: Gera relatórios financeiros ou administrativos.
- **`Usuario.java`**: Define as características e funcionalidades básicas de um usuário.

---

### **`utils`**
Contém utilitários auxiliares para o projeto:
- **`CSVExporter.java`**: Exporta dados do sistema para arquivos CSV.
- **`DBUtils.java`**: Contém métodos utilitários para interações com o banco de dados.

---

### **`view`**
Gerencia a interface do usuário e a interação com o sistema:
- **`CadastroView.java`**: Tela de cadastro de novos usuários, contas ou funcionários.
- **`ClienteView.java`**: Tela principal para interação com os clientes.
- **`FuncionarioView.java`**: Tela principal para interação com funcionários do banco.
- **`MainView.java`**: Tela inicial principal da aplicação.
- **`PasswordDialogView.java`**: Diálogo para autenticação via senha.
- **`WelcomeView.java`**: Tela de boas-vindas ao sistema.
