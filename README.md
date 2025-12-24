# 📈 InvestTrack

**InvestTrack** é uma plataforma financeira moderna desenvolvida para **monitoramento, análise e simulação de investimentos**, utilizando **dados econômicos oficiais do Brasil**.  
A aplicação integra múltiplas fontes governamentais e transforma dados públicos em **inteligência financeira acionável** para o investidor.

> Projeto focado em **renda fixa**, indicadores macroeconômicos e análises baseadas em dados reais.

---

## 🏛️ Fontes Oficiais de Dados

O InvestTrack consome dados diretamente de APIs governamentais confiáveis:

- **Banco Central do Brasil (SGS)**
  - Séries históricas da **SELIC**
  - Índices de inflação (**IPCA**)

- **Tesouro Nacional**
  - Preços e taxas atualizadas de **títulos públicos**

Essas integrações garantem **precisão, confiabilidade e atualização contínua** das informações.

---

## 🛠️ Stack Tecnológica

O projeto utiliza tecnologias modernas e consolidadas no ecossistema .NET:

- **Back-end:** ASP.NET Core Web API (.NET 8)
- **Front-end:** Blazor WebAssembly (Client-side)
- **Arquitetura:** Clean Architecture
- **Comunicação:** DTOs compartilhados para tipagem forte ponta-a-ponta
- **Integração Externa:** HttpClient para consumo de APIs governamentais
- **Cache:** Estratégias para redução de chamadas externas

---

## 🏗️ Arquitetura da Solução

A aplicação segue uma **organização em camadas**, priorizando manutenibilidade, testabilidade e escalabilidade:

   nvestTrack.Domain
├─ Entidades de negócio
├─ Value Objects
└─ Interfaces (contratos)

InvestTrack.Application
├─ Casos de uso
├─ Serviços de domínio
├─ Cálculos financeiros
└─ Regras de negócio

InvestTrack.Infrastructure
├─ Consumo de APIs externas
├─ Implementações de repositórios
├─ Cache e persistência
└─ Serviços técnicos

InvestTrack.Shared
├─ DTOs
├─ Enums
└─ Utilitários comuns

InvestTrack.API
├─ Endpoints (Controllers / Minimal APIs)
└─ Configuração da aplicação

InvestTrack.Client
└─ Interface de usuário em Blazor WebAssembly


---

## 🚀 Funcionalidades

- ✅ **Dashboard de Indicadores**
  - Visualização em tempo real de SELIC, IPCA e outros indicadores macroeconômicos.

- ✅ **Simulador de Renda Fixa**
  - Cálculo de juros compostos com base em **SELIC** e **CDI**.

- ✅ **Calculadora de Imposto de Renda (IR)**
  - Aplicação automática da **tabela regressiva** para renda fixa.

- 🚧 **Projeção de Inflação**
  - Comparação entre **ganho nominal x ganho real** (em desenvolvimento).

---

## 🎯 Objetivo do Projeto

O InvestTrack foi criado com o objetivo de:

- Democratizar o acesso a **dados financeiros oficiais**
- Facilitar a **tomada de decisão baseada em indicadores reais**
- Servir como **base para estudos, evolução para SaaS ou produto comercial**
- Aplicar boas práticas de **arquitetura limpa no ecossistema .NET**

---

## 📌 Status do Projeto

> 🧪 Em desenvolvimento ativo — novas funcionalidades e melhorias contínuas.
