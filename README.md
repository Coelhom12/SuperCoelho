# 🛒 Supermercado Coelho - Gestão e Otimização Financeira de Escalas

> **Projeto acadêmico (PAC VII - 2026/1) focado na geração, validação paramétrica e otimização de custos de escalas de trabalho para o setor varejista.**

![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow?style=for-the-badge)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-F2F4F9?style=for-the-badge&logo=spring-boot)
![Academic](https://img.shields.io/badge/Projeto-Universitário-blue?style=for-the-badge)

---

## 📖 Sobre o Projeto

A elaboração de escalas no setor de supermercados é um desafio complexo. Quando feita manualmente, frequentemente resulta em **subdimensionamento** (filas e mau atendimento) ou **superdimensionamento / overstaffing** (excesso de funcionários em dias de baixo movimento, gerando prejuízos silenciosos). 

Este sistema web foi idealizado para o **Supermercado Coelho** com o objetivo de ir além de um simples "calendário de turnos". Ele cruza restrições trabalhistas da CLT, dados salariais individuais (incluindo adicionais de domingos e feriados) e **projeções de faturamento diário** para garantir que a loja opere com a equipe exata, protegendo a margem de lucro.

---

## ✨ Principais Funcionalidades

*   **⚙️ Módulo Base de Cadastros:** Gerenciamento completo de setores, funcionários, variáveis salariais e regras sindicais/trabalhistas.
*   **🧠 Motor de Cálculo e Otimização Financeira:** Algoritmo inteligente que bloqueia ou emite alertas caso o custo da escala montada para o dia ultrapasse o teto financeiro viável baseado na projeção de renda.
*   **📅 Matriz de Escala Dinâmica:** Interface (Frontend) visual e interativa para alocação de funcionários com feedback e validação de regras em tempo real.
*   **🛡️ Auditoria de Conflitos:** Prevenção automática contra sobreposição de horários e desrespeito a regras de interjornada.

---

## 🧮 O Diferencial: Inteligência Financeira

O coração do sistema é o seu motor de validação. Ele calcula dinamicamente o custo da escala (`Salário/Hora × Horas Trabalhadas × Peso do Dia`) e garante que o número de operadores alocados seja:
1. Maior ou igual à necessidade mínima logística de atendimento.
2. **Menor ou igual** ao limite máximo suportável financeiramente pela loja naquele dia específico.

---

## 🛠️ Tecnologias Utilizadas (Arquitetura Preliminar)

A arquitetura do projeto é dividida entre Cliente e Servidor para garantir escalabilidade e manutenção. *(Nota: A stack pode sofrer adaptações ao longo do desenvolvimento prático).*

**Backend:**
*   ☕ **Java** - Linguagem principal.
*   🍃 **Spring Boot** - Criação ágil de APIs RESTful e injeção de dependências.
*   💾 **Spring Data JPA** - Mapeamento objeto-relacional e persistência de dados.

**Frontend / Infraestrutura:**
*   💻 **SPA (Single Page Application)** - Para renderização fluida da matriz de horários.
*   🔥 **Firebase** - Previsão de uso para autenticação moderna e hospedagem.

---

## 🚀 Como Executar o Projeto (Em breve)

*Instruções detalhadas serão adicionadas conforme a liberação das versões iniciais (Sprints).*

```bash
# Clone este repositório
git clone [https://github.com/SeuUsuario/supermercado-coelho-escalas.git](https://github.com/SeuUsuario/supermercado-coelho-escalas.git)

# Acesse a pasta do projeto
cd supermercado-coelho-escalas

# Comandos de execução do backend (Exemplo)
./mvnw spring-boot:run
