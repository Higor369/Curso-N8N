# Workflows N8N - Curso Udemy

Este repositório contém uma coleção de workflows do N8N desenvolvidos durante o curso de N8N da Udemy. Os workflows demonstram diferentes funcionalidades e integrações do N8N para automação de processos.

## 📋 Sobre o Projeto

Este projeto é uma compilação de workflows práticos criados durante o aprendizado do N8N, uma ferramenta poderosa de automação de workflows que permite conectar diferentes serviços e APIs de forma visual e intuitiva.

## 🗂️ Estrutura do Projeto

```
n8n/
├── Modulo-1/
│   ├── primeiro workflow.json
│   └── Segundo workflow.json
└── README.md
```

## 📚 Módulos

### Módulo 1 - Workflows de Automação

#### 1. Formulário de Contato com Integração

**Arquivo:** `Modulo-1/primeiro workflow.json`

**Descrição:** Workflow que demonstra a criação de um formulário de contato com integração ao Google Sheets e envio de email via Gmail.

**Funcionalidades:**
- 📝 Formulário web com campos personalizados (Nome, Idade, Cidade, Escolaridade)
- 📊 Armazenamento automático dos dados no Google Sheets
- 📧 Envio de notificação por email com os dados do formulário

**Componentes do Workflow:**
1. **Form Trigger** - Captura dados do formulário web
2. **Google Sheets** - Armazena dados em planilha
3. **Gmail** - Envia notificação por email

**Campos do Formulário:**
- Nome (obrigatório)
- Idade (obrigatório, numérico)
- Cidade (obrigatório)
- Escolaridade (obrigatório, dropdown: Fundamental, Médio, Superior)

#### 2. Monitoramento de Planilha com Notificações

**Arquivo:** `Modulo-1/Segundo workflow.json`

**Descrição:** Workflow que monitora uma planilha do Google Sheets e executa múltiplas ações quando uma nova linha é adicionada.

**Funcionalidades:**
- 🔍 Monitoramento automático de planilha (verificação a cada minuto)
- 💬 Notificação no Slack quando novo registro é inserido
- 📧 Envio de email personalizado para o usuário
- 👤 Criação automática de contato no Google Contacts

**Componentes do Workflow:**
1. **Google Sheets Trigger** - Monitora adição de novas linhas
2. **Slack** - Envia notificação no canal
3. **Gmail** - Envia email para o usuário
4. **Google Contacts** - Cria contato automaticamente

**Campos Monitorados:**
- Nome
- Descrição
- Email
- Telefone

## 🚀 Como Usar

### Pré-requisitos
- Conta N8N (cloud ou self-hosted)
- Conta Google (para Google Sheets, Gmail e Google Contacts)
- Conta Slack (para notificações)
- Credenciais configuradas no N8N

### Importação dos Workflows

1. Acesse sua instância do N8N
2. Vá para a seção "Workflows"
3. Clique em "Import from File"
4. Selecione o arquivo `.json` do workflow desejado
5. Configure as credenciais necessárias
6. Ative o workflow

### Configuração de Credenciais

Para os workflows do Módulo 1, você precisará configurar:

**Primeiro Workflow:**
- **Google Sheets OAuth2**: Para acessar e modificar planilhas
- **Gmail OAuth2**: Para envio de emails

**Segundo Workflow:**
- **Google Sheets Trigger OAuth2**: Para monitorar planilhas
- **Slack OAuth2**: Para envio de mensagens
- **Gmail OAuth2**: Para envio de emails
- **Google Contacts OAuth2**: Para criação de contatos

## 🔧 Tecnologias Utilizadas

- **N8N** - Plataforma de automação de workflows
- **Google Sheets API** - Integração com planilhas
- **Gmail API** - Envio de emails
- **Google Contacts API** - Gerenciamento de contatos
- **Slack API** - Notificações em canais
- **Form Trigger** - Captura de dados de formulários web
- **Google Sheets Trigger** - Monitoramento de planilhas

## 📖 Conceitos Aprendidos

- Criação de formulários web com N8N
- Integração com Google Workspace (Sheets, Gmail e Contacts)
- Integração com Slack para notificações
- Mapeamento de dados entre diferentes serviços
- Configuração de triggers e webhooks
- Monitoramento automático de planilhas
- Automação de processos de coleta e notificação de dados
- Criação automática de contatos
- Workflows reativos baseados em eventos

## 🎯 Objetivos do Curso

Este projeto tem como objetivo demonstrar:

1. **Automação de Processos**: Como automatizar tarefas repetitivas
2. **Integração de Serviços**: Conectar diferentes plataformas
3. **Coleta de Dados**: Capturar informações de usuários
4. **Monitoramento**: Acompanhar mudanças em tempo real
5. **Notificações**: Enviar alertas e confirmações
6. **Armazenamento**: Salvar dados de forma organizada
7. **Gestão de Contatos**: Criação automática de contatos
8. **Comunicação**: Integração com ferramentas de comunicação

## 📝 Próximos Passos

Conforme o curso avança, novos módulos serão adicionados com workflows mais complexos, incluindo:

- Integrações com APIs externas
- Processamento de dados
- Workflows condicionais
- Automações avançadas

## 🤝 Contribuições

Este é um projeto de aprendizado pessoal. Sinta-se à vontade para:

- Sugerir melhorias nos workflows
- Reportar problemas ou bugs
- Compartilhar suas próprias implementações

## 📄 Licença

Este projeto é para fins educacionais e de aprendizado.

---

**Desenvolvido durante o curso de N8N da Udemy** 🎓
