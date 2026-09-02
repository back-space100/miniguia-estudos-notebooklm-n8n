# miniguia-estudos-notebooklm-n8n
Projeto DIO: Caderno Temático no NotebookLM como Tutor de Automação com n8n e Portfólio.

# 🤖 Miniguia de Estudos: Automação com n8n e Portfólio (NotebookLM)

> Projeto desenvolvido para o desafio da plataforma **DIO (Digital Innovation One)** com foco em aprendizagem ativa e curadoria de conhecimento via Inteligência Artificial.

---

## 🎯 1. Contexto e Objetivos

* **Tema Escolhido:** Automação de Processos com n8n e construção de projetos práticos para portfólio back-end.
* **Objetivo de Estudo:** Utilizar o NotebookLM como um tutor personalizado para acelerar a conclusão do curso de automação com n8n, compreender conceitos avançados (Webhooks, requisições HTTP, nós de código) e gerar documentações padronizadas de projetos para o GitHub.

---

## 📚 2. Curadoria de Fontes

Para alimentar a base do NotebookLM e atuar como nosso tutor, foram selecionadas e inseridas 4 fontes focadas em conceitos práticos, integrações e boas práticas de portfólio:

1. **Plano de Estudos e Fundamentos de n8n:** Guia conceitual sobre arquitetura orientada a nós, tipos de nós principais (Webhook, HTTP Request, Code, IF) e boas práticas de automação.
2. **Guia de Integração (Webhooks e APIs REST):** Documentação técnica abordando comunicação orientada a eventos, rotas HTTP, autenticação de APIs e manipulação de payloads JSON.
3. **Diretrizes para Projetos de Portfólio com n8n:** Roteiro prático com sugestões de projetos reais de automação (notificadores, enriquecimento de dados) e estrutura padrão para documentação no GitHub.
4. **Guia de Versionamento com Git e GitHub:** Referência técnica sobre fluxo de comandos Git (`commit`, `push`), organização do repositório e padrões de documentação em Markdown.

---

## 🛠️ 3. Engenharia de Prompts e Solução de Problemas (Troubleshooting)

Abaixo estão registrados os testes de prompts efetuados no NotebookLM, demonstrando o processo iterativo de refatoração das perguntas para extrair respostas mais precisas e técnicas da base de conhecimento ("Cicatrizes de Aprendizado"):

### 🔬 Teste 1: Sugestão de Projeto para Portfólio
* **Prompt Inicial (Genérico):** *"Me dá uma ideia de projeto no n8n."*
* **Dificuldade / Ponto Cego:** Resposta vaga e sem direcionamento para portfólio profissional ou estrutura de repositório.
* **Prompt Refinado:** *"Com base no documento de Diretrizes para Projetos de Portfólio, sugira um projeto prático que combine o uso do nó Webhook com envio de mensagens no n8n. Explique detalhadamente o problema resolvido e quais itens devem constar no README do projeto no GitHub."*
* **Resultado Obtido:** A IA utilizou a Fonte 3 da curadoria para sugerir o *Notificador Automático de Logs*, detalhando exatamente como estruturar o repositório do projeto.

---

### 🔬 Teste 2: Esclarecimento de Conceito Técnico (Webhook vs HTTP Request)
* **Prompt Inicial (Genérico):** *"Qual a diferença de Webhook para HTTP Request?"*
* **Dificuldade / Ponto Cego:** Resposta puramente acadêmica sem aplicação prática no contexto do n8n.
* **Prompt Refinado:** *"Com base no Guia de Integração de Webhooks e APIs REST, explique em linguagem simples e com um exemplo prático a diferença entre o nó Webhook e o nó HTTP Request no n8n. Em que momento devo usar cada um num fluxo de automação?"*
* **Resultado Obtido:** Resposta contextualizada citando a Fonte 2, diferenciando eventos passivos (Webhook) de requisições ativas a APIs externas (HTTP Request).

---

### 🔬 Teste 3: Geração de Template de Documentação
* **Prompt Inicial (Genérico):** *"Como faço um README para meu projeto de n8n?"*
* **Dificuldade / Ponto Cego:** Falta de padrões específicos para projetos de automação de processos.
* **Prompt Refinado:** *"Atuando como um tutor especializado em n8n e Git, gere um template em Markdown de README.md para um projeto de automação do n8n. O template deve conter as seções: Descrição do Problema, Fluxo de Nós Utilizados, Como Importar o JSON e Teste com Webhook."*
* **Resultado Obtido:** Síntese cruzada entre a Fonte 3 e a Fonte 4 gerando um template completo em Markdown pronto para ser reutilizado.
  
---

## 📖 4. Miniguia de Estudo (Entrega Final)

### 📌 Resumo Estruturado do Assunto
O **n8n** é uma plataforma de automação baseada em workflows e nós (nodes) interconectados. Para criar projetos relevantes para o mercado de back-end:
* **Entrada de Dados:** A automação inicia-se com gatilhos ativos ou passivos. O nó `Webhook` aguarda notificações HTTP disparadas em tempo real por aplicações externas (como sistemas em Java/Spring Boot).
* **Processamento e Regras:** O nó `Code` permite executar lógica em JavaScript ou Python para tratar dados JSON complexos, enquanto nós como `IF` e `Switch` direcionam o fluxo de acordo com validações condicionais.
* **Saída e Integração:** Através do nó `HTTP Request`, o fluxo pode consumir rotas REST de terceiros, salvar registros em bancos PostgreSQL ou emitir notificações instantâneas em canais de comunicação.
* **Versionamento e Portfólio:** Todos os fluxos criados podem ser exportados no formato JSON e mantidos em repositórios no GitHub acompanhados de documentação detalhada (README.md) e instrução de consumo.

---

### 📚 Glossário de Conceitos-Chave

| Conceito | Descrição Prática |
| :--- | :--- |
| **n8n** | Ferramenta open-source e expansível para automação de processos baseada em nós. |
| **Webhook** | Ponto de entrada que recebe requisições de eventos disparados por outros sistemas em tempo real. |
| **HTTP Request** | Nó utilizado para consumir ou enviar dados a APIs REST externas via métodos HTTP (GET, POST, PUT, DELETE). |
| **Payload JSON** | Estrutura de dados em formato de texto trocada entre o n8n e os sistemas integrados. |
| **Node (Nó)** | Bloco individual do fluxo do n8n responsável por executar uma ação ou regra específica. |
| **Workflow** | Sequência lógica de nós interligados que resolvem um processo de ponta a ponta. |

---

### 💡 Prompts Reutilizáveis para Estudos Futuros

Abaixo está o gabarito de prompts validados para apoiar futuras revisões e novos projetos:

1. **Revisão Conceitual Rápidas:**
   > *"Atue como um especialista em n8n e explique a diferença prática entre os nós [Nome do Nó A] e [Nome do Nó B], dando um exemplo do mundo real de quando usar cada um."*
2. **Planejamento de Novo Projeto de Portfólio:**
   > *"Preciso criar uma automação no n8n para [Problema de Negócio]. Quais nós devo colocar em sequência e como devo estruturar a entrada de dados via Webhook?"*
3. **Criação de Documentação para GitHub:**
   > *"Gere a estrutura de um README.md em Markdown para o projeto de automação [Nome do Projeto], incluindo o passo a passo de como importar o arquivo JSON no n8n e como testar com o Postman."*
