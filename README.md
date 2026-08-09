# 🤖 Agente de IA para Clínica Médica

Agente de Inteligência Artificial desenvolvido para automatizar o atendimento de pacientes de uma clínica médica através do **WhatsApp**.

O agente atua como uma secretária virtual, conduzindo conversas de forma natural e auxiliando pacientes no agendamento, reagendamento e cancelamento de consultas e serviços da clínica.

## 🚀 Funcionalidades

* 💬 Atendimento automatizado via WhatsApp
* 🤖 Conversação com Inteligência Artificial
* 🧠 Memória das conversas utilizando Redis
* 📅 Agendamento de consultas
* 🔄 Reagendamento de consultas
* ❌ Cancelamento de consultas
* 📆 Verificação de disponibilidade de horários
* 📧 Coleta de dados do paciente
* 🩺 Apresentação dos serviços da clínica
* 🔒 Regras para evitar diagnósticos e orientações médicas indevidas

## 🛠️ Tecnologias utilizadas

* **n8n** — Automação e orquestração do agente
* **AI Agent** — Processamento das conversas
* **Groq / LLM** — Inteligência Artificial
* **Redis** — Memória conversacional
* **Evolution API** — Integração com WhatsApp
* **Google Calendar** — Gerenciamento dos agendamentos
* **Webhooks** — Comunicação entre os serviços

## 🔄 Fluxo do agente

```text
WhatsApp
    ↓
Evolution API
    ↓
Webhook
    ↓
n8n
    ↓
Processamento da mensagem
    ↓
Memória Redis
    ↓
AI Agent
    ↓
Google Calendar
    ↓
Evolution API
    ↓
WhatsApp
```

## 📅 Gerenciamento de consultas

O agente consegue:

1. Identificar a intenção do paciente.
2. Solicitar somente as informações necessárias.
3. Verificar a disponibilidade no Google Calendar.
4. Confirmar os dados antes do agendamento.
5. Criar o evento no calendário.
6. Reagendar consultas existentes.
7. Cancelar consultas existentes.
8. Enviar a confirmação ao paciente pelo WhatsApp.

## 🧠 Memória

O agente utiliza **Redis** para manter o contexto das conversas.

Isso permite que o paciente forneça as informações aos poucos sem precisar repetir dados que já foram informados anteriormente.

## ⚠️ Segurança

O agente não realiza diagnósticos médicos nem fornece orientações clínicas.

Quando o paciente apresenta uma dúvida médica, o atendimento é direcionado para avaliação do profissional responsável.

## 🎯 Objetivo do projeto

Este projeto demonstra a aplicação de **Agentes de IA e automações no atendimento de clínicas médicas**, reduzindo tarefas repetitivas e permitindo que a equipe se concentre no atendimento aos pacientes.

---

### 👨‍💻 Desenvolvido por Matheus Pacheco

Projeto desenvolvido como parte do portfólio de soluções de **Automação e Inteligência Artificial**.
