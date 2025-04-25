# Exemplo de Estrutura Inicial para Knowledge Graph

Este documento apresenta um exemplo de como estruturar as informações iniciais para o Knowledge Graph, servindo como ponto de partida para implementação do sistema de memória.

## Entidades Principais

```json
[
  {
    "name": "Pedro",
    "entityType": "pessoa",
    "observations": [
      "Tem 22 anos",
      "Mora em Itu/SP, Brasil",
      "Trabalha com marketing digital",
      "Empreendedor com experiência em vários nichos",
      "Gerencia marketing para D'Ajuda Refeições",
      "Fundador conceitual da Aura[IA] Marketing",
      "Perfil DISC: C (28 pontos), D (25 pontos), S (22 pontos), I (15 pontos)",
      "Enfrenta desafios com procrastinação e paralisia por análise",
      "Aprecia jogos e tecnologia",
      "Busca crescimento financeiro e profissional",
      "Sonha com casa própria para viver com Gabi e Lola",
      "Mantra pessoal: 'A procrastinação só vai te vencer, até o PIX vencer a procrastinação'"
    ]
  },
  {
    "name": "Aura[IA]_Marketing",
    "entityType": "projeto",
    "observations": [
      "Agência de marketing digital focada em IA",
      "Fundada conceitualmente por Pedro",
      "Mantra: 'Iluminar conexões, transformar realidades'",
      "Diferencial: abordagem que combina inteligência humana e IA",
      "Identidade visual baseada na aurora boreal",
      "Cores principais: roxo, azul e turquesa",
      "Em fase inicial de desenvolvimento",
      "Modelo de negócio: One Person Business com alto nível de automação"
    ]
  },
  {
    "name": "Performance_AI",
    "entityType": "serviço",
    "observations": [
      "Serviço da Aura[IA] Marketing",
      "Análise avançada de campanhas de marketing digital",
      "Identifica problemas e oportunidades ocultas",
      "Combina habilidades analíticas naturais de Pedro com IA",
      "Preço da análise completa: R$597",
      "Oferece análise inicial gratuita como estratégia de entrada",
      "Landing page: performanceai.my.canva.site",
      "Em fase de validação inicial"
    ]
  },
  {
    "name": "D'Ajuda_Refeições",
    "entityType": "empresa",
    "observations": [
      "Negócio de marmitas de Maria Gabriela (Gabi)",
      "Pedro trabalha como gestor de marketing",
      "Localização: R. Vinte e Quatro de Fevereiro, 54 - Vila Nova, Itu/SP",
      "Carro-chefe: 'Marmita de Itu' (1kg a 1,5kg)",
      "Atua em Itu e Salto (SP)",
      "Proposta de valor: comida caseira em quantidade generosa",
      "Cardápio rotativo diário",
      "Instagram: @dajudarefeicoes",
      "Contato principal: WhatsApp (11) 99536-0847"
    ]
  },
  {
    "name": "Bestiário_IA_Brasileira",
    "entityType": "projeto",
    "observations": [
      "Conteúdo criativo para comunidade de IA",
      "Analisa de forma humorística o marketing de IA no Brasil",
      "Categoriza 'espécies' de vendedores e usuários de IA",
      "Formato de bestiário científico vintage",
      "Co-criado por Pedro e Aura",
      "Inclui ilustrações no estilo de manual científico",
      "Tom humorístico com insights reais sobre o mercado"
    ]
  },
  {
    "name": "Inventário_RPG_Notion",
    "entityType": "projeto",
    "observations": [
      "Template para visualizar jornada de aprendizado em IA no formato de inventário de RPG",
      "Inspirado em jogos como Dead Space e Cyberpunk",
      "Usa estética sci-fi com tons roxos/azuis",
      "Categoriza conhecimentos como 'itens' de diferentes raridades",
      "Inclui sistema de 'estatísticas de personagem' para acompanhar progresso",
      "Objetivo: gamificar e visualizar desenvolvimento pessoal",
      "Em fase de desenvolvimento"
    ]
  },
  {
    "name": "Claude",
    "entityType": "ferramenta_ia",
    "observations": [
      "Assistente de IA da Anthropic",
      "Modelo preferido para conversas aprofundadas",
      "Usado para brainstorming e desenvolvimento de conceitos",
      "Considerado parceiro na criação da Aura[IA]",
      "Capacidades expandidas recentemente com MCP (Model Context Protocol)"
    ]
  },
  {
    "name": "Gabi",
    "entityType": "pessoa",
    "observations": [
      "Maria Gabriela, namorada de Pedro",
      "Dona da D'Ajuda Refeições",
      "Oferece apoio emocional e profissional a Pedro",
      "Compartilha sonho de ter casa própria com Pedro"
    ]
  },
  {
    "name": "Lola",
    "entityType": "animal",
    "observations": [
      "Coelhinha de estimação de Pedro",
      "Pedro tem imenso amor e preocupação por ela",
      "Atualmente vive com Gabi",
      "Parte importante da 'família' que Pedro quer construir"
    ]
  }
]
```

## Relações Iniciais

```json
[
  {
    "from": "Pedro",
    "to": "Aura[IA]_Marketing",
    "relationType": "fundou"
  },
  {
    "from": "Pedro",
    "to": "D'Ajuda_Refeições",
    "relationType": "trabalha_para"
  },
  {
    "from": "Pedro",
    "to": "Performance_AI",
    "relationType": "desenvolveu"
  },
  {
    "from": "Pedro",
    "to": "Bestiário_IA_Brasileira",
    "relationType": "criou"
  },
  {
    "from": "Pedro",
    "to": "Inventário_RPG_Notion",
    "relationType": "está_desenvolvendo"
  },
  {
    "from": "Pedro",
    "to": "Claude",
    "relationType": "utiliza"
  },
  {
    "from": "Pedro",
    "to": "Gabi",
    "relationType": "namora_com"
  },
  {
    "from": "Pedro",
    "to": "Lola",
    "relationType": "é_dono_de"
  },
  {
    "from": "Gabi",
    "to": "D'Ajuda_Refeições",
    "relationType": "é_proprietária_de"
  },
  {
    "from": "Gabi",
    "to": "Lola",
    "relationType": "cuida_de"
  },
  {
    "from": "Aura[IA]_Marketing",
    "to": "Performance_AI",
    "relationType": "oferece"
  },
  {
    "from": "Performance_AI",
    "to": "D'Ajuda_Refeições",
    "relationType": "pode_otimizar"
  }
]
```

## Estrutura para Implementação

Este modelo JSON pode ser utilizado diretamente com as ferramentas do MCP Memory:

1. Use `create_entities` para adicionar todas as entidades listadas
2. Use `create_relations` para estabelecer as conexões entre entidades
3. Use `add_observations` para atualizar entidades com novas informações

À medida que novas informações surgem nas conversas, o grafo pode ser expandido usando:

```javascript
// Exemplo de adição de nova entidade
await memory.create_entities([
  {
    name: "Nome_Projeto",
    entityType: "projeto",
    observations: ["Descrição", "Objetivo", "Status"]
  }
]);

// Exemplo de criação de relação
await memory.create_relations([
  {
    from: "Pedro",
    to: "Nome_Projeto",
    relationType: "está_trabalhando_em"
  }
]);

// Exemplo de adição de observações
await memory.add_observations([
  {
    entityName: "Pedro",
    contents: ["Nova informação descoberta"]
  }
]);
```

Este modelo inicial servirá como base para a construção gradual de um grafo de conhecimento personalizado que captura não apenas fatos, mas também conexões, padrões e insights sobre o usuário e seu contexto.