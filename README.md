# Claude Memory System

![Memory System](https://img.shields.io/badge/MCP-Knowledge%20Graph-8A2BE2)

Um sistema de memória persistente para Claude baseado em Knowledge Graph, proporcionando interações mais contextualizadas e personalizadas.

## 📝 Visão Geral

Este repositório contém a estrutura e documentação para implementar um sistema de memória persistente para Claude, permitindo que o assistente mantenha informações contextuais entre conversas. O sistema utiliza um Knowledge Graph para armazenar e relacionar informações de forma estruturada.

## 🧠 Como Funciona

O sistema utiliza o Model Context Protocol (MCP) para implementar um servidor de memória que:

1. Armazena informações em um grafo de conhecimento
2. Mantém entidades, suas propriedades e relações entre elas
3. Permite consultas e atualizações dinâmicas
4. Preserva o contexto entre diferentes sessões de conversa

## 📂 Estrutura do Repositório

- `memoria_claude.md` - Instruções de funcionamento do sistema de memória
- `questionario_perfil_pessoal.md` - Questionário para mapear informações pessoais e cognitivas
- `casos_de_uso_memory_graph.md` - Casos de uso práticos do sistema para aprendizes de IA
- `exemplo_estrutura_inicial.md` - Exemplo de estrutura inicial para o Knowledge Graph

## 🚀 Casos de Uso Principais

O sistema de memória foi desenvolvido principalmente para:

1. **Mapear a jornada de aprendizado em IA**
2. **Acompanhar ideias e projetos**
3. **Manter uma biblioteca pessoal de prompts**
4. **Rastrear conexões entre projetos**
5. **Gerenciar relacionamentos profissionais**
6. **Facilitar reflexão e metacognição**
7. **Combater procrastinação e paralisia por análise**
8. **Mapear padrões cognitivos**

## 🛠️ Implementação Técnica

O sistema utiliza a API do Knowledge Graph para:

- Criar entidades (`create_entities`)
- Estabelecer relações (`create_relations`)
- Adicionar observações (`add_observations`)
- Consultar o grafo (`read_graph`, `search_nodes`, `open_nodes`)
- Modificar e atualizar elementos (`delete_entities`, `delete_observations`, `delete_relations`)

## 🔮 Benefícios

- **Continuidade:** Interações que mantêm contexto ao longo do tempo
- **Personalização:** Respostas adaptadas ao seu perfil específico
- **Estruturação:** Transformação de informações caóticas em conhecimento organizado
- **Metacognição:** Facilitação da reflexão sobre padrões de pensamento e comportamento
- **Produtividade:** Redução da sobrecarga cognitiva e paralisia por análise

## 🌱 Primeiros Passos

1. Preencha o questionário de perfil pessoal
2. Revise e adapte o exemplo de estrutura inicial
3. Escolha os casos de uso mais relevantes para você
4. Implemente o sistema usando um servidor MCP de Knowledge Graph

## 👁️ Privacidade

Todas as informações são armazenadas localmente no servidor MCP, garantindo privacidade e controle sobre seus dados.

---

*"A procrastinação só vai te vencer, até o PIX vencer a procrastinação"*