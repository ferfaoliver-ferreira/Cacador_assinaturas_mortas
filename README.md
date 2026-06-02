# 🎯 Caçador de Assinaturas Mortas

![Status do Projeto](https://img.shields.io/badge/Status-Conceito%20%2F%20MVP-brightgreen)
![Tecnologias](https://img.shields.io/badge/Foco-Open%20Banking%20%7C%20Data%20%7C%20UX-blue)

O **Caçador de Assinaturas Mortas** é uma solução de inteligência financeira e de dados desenvolvida para combater o desperdício invisível: assinaturas de serviços (streamings, aplicativos, clubes de benefícios) que o usuário continua pagando, mas não utiliza mais. 

O projeto foi concebido sob a metodologia ágil (Scrum/Sprints rápidos) durante um desafio de gestão de projetos e desenvolvimento pessoal.


<img width="1335" height="538" alt="image" src="https://github.com/user-attachments/assets/1bc09692-4f7b-432c-8a06-c62ae9e25c33" />


---

## 📱 A Interface do Usuário

<p align="center">
  <img width="740" height="1600" alt="interface caçador de assinaturas mortas" src="https://github.com/user-attachments/assets/adbf7ec6-a7d3-4c74-b696-4d69ee90965e" />

</p>

---

## 💡 O Problema
Estudos de mercado mostram que uma parcela significativa dos consumidores possui "vazamentos financeiros" silenciosos na conta bancária. O esquecimento de cancelar avaliações gratuitas (*free trials*) ou a perda de interesse em serviços recorrentes geram um gasto acumulado que passa despercebido no dia a dia.

<img width="1335" height="626" alt="Captura de tela 2026-06-01 212709" src="https://github.com/user-attachments/assets/0e0a6d6c-0ceb-4994-8089-cc69aa6994ca" />


## 🚀 A Solução e Diferenciais
A proposta do aplicativo elimina a complexidade das planilhas de gastos tradicionais, focando em automação e ação direta:

1. **Conexão via Open Banking:** Integração segura para leitura e varredura do histórico de transações bancárias e faturas de cartão de crédito.
2. **Identificação de "Assinaturas Mortas":** Cruzamento inteligente de dados de pagamento com o comportamento/histórico de uso do usuário (ex: detectar que o serviço está contratado, mas não registra atividade há mais de 60 ou 90 dias).
3. **Cancelamento com 1 Clique:** Automação do fluxo burocrático de cancelamento diretamente pela interface do app, utilizando APIs integradas com segurança.

<img width="1337" height="613" alt="image" src="https://github.com/user-attachments/assets/8fb5e933-b9a8-4548-b819-be10c1318491" />

---

## 📈 Visão de Negócio
<img width="1335" height="578" alt="Captura de tela 2026-06-01 215147" src="https://github.com/user-attachments/assets/d8b03dba-1254-4f0d-b9f8-9caa659ad471" />


## 🛠️ Arquitetura de Dados Proposta (Visão Conceitual)

O fluxo de funcionamento do ecossistema baseia-se em 4 etapas principais:

```text
[Instituição Financeira] 
       │ (Open Banking API)
       ▼
[Ingestão de Dados] ──► [Pipeline de Análise] ──► [Identificação Automatizada] ──► [Ação de Cancelamento]
                           (Identifica padrões       (Gera alerta de "Assinatura       (API de automação /
                            de recorrência)                 Morta")                     resolução de 1-clique)



       [ Camada 3: B2B2C ] ──► Parcerias com Bancos, Fintechs e Apps de Educação
                ▲
     [ Camada 2: Premium ] ──► Alertas Inteligentes, Central e Histórico Mensal
                ▲
    [ Camada 1: Freemium ] ──► Detecção Base e Visualização de Desperdício


