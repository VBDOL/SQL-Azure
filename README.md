# 📌 Configurando uma Instância de Banco de Dados Gerenciado no Microsoft Azure

## 🚀 Introdução
Este repositório documenta o processo de **configuração de uma Instância Gerenciada de SQL no Azure**. Aqui você encontrará resumos, anotações e dicas sobre o uso do **Microsoft Azure** para armazenamento e gerenciamento de dados.

---

## 🎯 Objetivos de Aprendizagem
Ao concluir este desafio, você será capaz de:
- Aplicar os conceitos aprendidos em um ambiente prático.
- Documentar processos técnicos de forma clara e estruturada.
- Utilizar o **GitHub** como ferramenta para compartilhamento de documentação técnica.

---

## 🏗️ Passos para Criar uma Instância Gerenciada de SQL no Azure

### 1️⃣ **Entrando no Portal do Azure**
- Acesse o [Portal do Azure](https://portal.azure.com).
- Faça login com sua **Conta Microsoft**.

### 2️⃣ **Criando a Instância Gerenciada de SQL**
1. No menu esquerdo do portal, selecione **SQL do Azure**.
2. Caso não encontre essa opção, clique em **Todos os Serviços** e pesquise por **SQL do Azure**.
3. Clique em **+ Criar** e selecione **Instância única** na lista suspensa.
4. Clique em **Criar** para abrir a página de configuração.

### 3️⃣ **Configurações Básicas**
Preencha as informações obrigatórias na guia **Básico**:
```
| Configuração | Valor sugerido | Descrição |
|-------------|---------------|-----------|
| **Assinatura** | Sua assinatura | Permissão para criação de recursos. |
| **Grupo de Recursos** | Novo ou existente | Organização de recursos no Azure. |
| **Nome da Instância** | Qualquer nome válido | Nome único para sua instância SQL. |
| **Região** | Escolha uma região | Onde será hospedada sua instância. |
| **Método de Autenticação** | Autenticação SQL | Pode ser combinada com Microsoft Entra. |
| **Logon de Administrador** | Nome de usuário válido | Não pode ser `serveradmin`. |
| **Senha** | Senha forte | Mínimo de 16 caracteres com requisitos de complexidade. |
```
### 4️⃣ **Configurando Computação e Armazenamento**
Clique em **Configurar Instância Gerenciada** e ajuste as seguintes configurações:
```
| Configuração | Valor sugerido | Descrição |
|-------------|---------------|-----------|
| **Camada de Serviço** | Uso Geral | Adequado para cargas de trabalho padrão. |
| **Geração do Hardware** | Série Standard (Gen5) | Padrão para instâncias SQL. |
| **vCores** | 8 vCores (padrão) | Define a capacidade de processamento. |
| **Armazenamento (GB)** | Valor ajustável | Dependendo da necessidade da aplicação. |
| **Licença do SQL Server** | Pagamento conforme o uso | Alternativamente, Benefício Híbrido do Azure. |
| **Redundância do Armazenamento** | Geográfica | Para segurança dos backups. |
```
### 5️⃣ **Definição de Rede**
- Criar ou usar uma **rede virtual existente**.
- Escolher o **tipo de conexão adequado**.
- Habilitar ou desabilitar **ponto de extremidade público**.

### 6️⃣ **Revisão e Criação**
- Após revisar todas as configurações, clique em **Revisar + Criar**.
- Aguarde a implantação da instância no grupo de recursos.
- Após a conclusão, vá até **SQL do Azure** para gerenciar sua instância.

---

## 📂 Organização do Repositório
- `README.md` 
---

## 📢 Reflexão
Este repositório serve como um guia prático para a **configuração de uma Instância Gerenciada de SQL no Azure**. A documentação clara e detalhada facilita o aprendizado e futuras referências!

