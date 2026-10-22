# Saldoo

Sistema de gestão financeira pessoal baseado em Inteligência Artificial Conversacional e Gamificação.

## Links

- **Aplicação:** https://screenshot-to-silk-94.lovable.app
- **Repositório:** https://github.com/viniciuscastroab-lgtm/dio-lab-vibe-coding-app-financas

## Demonstração

dashboard.png

O Saldoo foi desenvolvido com o objetivo de simplificar o controle financeiro através de uma experiência baseada em linguagem natural, permitindo que usuários registrem receitas, despesas, acompanhem metas financeiras e recebam orientações inteligentes de forma intuitiva.

---

## Contexto do Projeto

Este projeto foi desenvolvido como parte de um desafio da DIO (Digital Innovation One) com foco em aprendizado de Vibecoding, prototipação rápida e utilização de Inteligência Artificial no processo de desenvolvimento de software.

O desafio propunha a criação de uma aplicação utilizando IA como ferramenta de apoio para definição de requisitos, geração de ideias e construção do produto.

A proposta inicial foi fornecida durante o desafio, mas o projeto foi refinado ao longo do processo de desenvolvimento com novas ideias, funcionalidades e regras de negócio adicionadas por iniciativa própria, resultando na criação do Saldoo.

É importante destacar que esta aplicação se encontra em fase inicial de desenvolvimento (MVP) e foi construída com fins educacionais e de experimentação. Diversas funcionalidades ainda podem ser evoluídas, refinadas e melhor estruturadas em versões futuras.

---

## Sobre o Projeto

Grande parte das pessoas abandona aplicativos financeiros porque eles exigem preenchimento manual constante, formulários extensos e pouca personalização.

O Saldoo busca resolver esse problema oferecendo uma experiência conversacional, onde o usuário interage com um assistente financeiro para registrar movimentações, visualizar informações financeiras e acompanhar objetivos pessoais.

Além disso, o sistema utiliza conceitos de gamificação para incentivar hábitos financeiros mais saudáveis através de níveis, missões, conquistas e evolução pessoal.

---

## Principais Funcionalidades

### Registro Financeiro por Conversa

O usuário pode registrar movimentações utilizando linguagem natural.

Exemplos:

```text
Recebi salário de R$ 5.000

Ganhei R$ 750 de freelance

Gastei R$ 45 no mercado

Uber R$ 18
```

---

### Gestão de Receitas

Categorias de entrada:

- Salário
- Benefícios
- Vale Alimentação
- Vale Refeição
- Auxílio Combustível
- Freelancer
- Diárias
- Investimentos
- Aluguéis
- Outros

---

### Gestão de Despesas

Classificação automática das despesas:

- Alimentação
- Transporte
- Moradia
- Saúde
- Educação
- Compras
- Lazer
- Assinaturas
- Investimentos
- Outros

---

### Cofres Financeiros

O sistema permite a criação de reservas financeiras para objetivos específicos.

Exemplos:

- Reserva de Emergência
- Viagem
- Casa Própria
- Novo Veículo
- Estudos

Exemplo de uso:

```text
Criar reserva viagem com meta de R$ 5.000
```

Regra implementada:

Quando um valor é transferido para um Cofre, ele deixa de fazer parte do saldo disponível principal.

Exemplo:

```text
Saldo disponível: R$ 3.000

Transferência para Cofre Viagem: R$ 500

Novo saldo disponível: R$ 2.500

Cofre Viagem: R$ 500 / R$ 5.000
```

Essa abordagem simula de forma mais realista a separação do dinheiro destinado aos objetivos financeiros.

---

### Gamificação

O Saldoo transforma a organização financeira em uma jornada de evolução.

Recursos:

- Sistema de XP
- Sistema de níveis
- Missões diárias
- Missões semanais
- Conquistas
- Progressão financeira

Exemplos de níveis:

- Aprendiz Financeiro
- Organizador de Orçamento
- Investidor Iniciante
- Estrategista Financeiro
- Lenda Financeira

---

### Chefes Financeiros

O sistema identifica automaticamente gastos recorrentes.

Exemplos:

- Netflix
- Spotify
- Amazon Prime
- Academia
- Internet
- Plano de Saúde

Esses gastos são apresentados como "Chefes Financeiros", permitindo ao usuário visualizar melhor o impacto dos custos fixos em seu orçamento.

---

### Indicadores Financeiros

- Saúde Financeira
- Taxa de Economia
- Índice de Evolução
- Índice de Impulsividade
- Estabilidade Financeira

---

## Tecnologias Utilizadas

- React
- TypeScript
- Tailwind CSS
- Supabase
- Shadcn/UI
- OpenAI (estrutura preparada para integração)
- Vercel

---

## Processo de Construção com IA

O projeto foi desenvolvido utilizando Inteligência Artificial como apoio para definição de produto, refinamento de requisitos e evolução das funcionalidades.

Durante a criação do Saldoo foi utilizado um processo iterativo de engenharia de prompts para transformar a ideia inicial em um produto mais completo e estruturado.

A IA auxiliou na definição de:

- Estrutura do MVP
- Funcionalidades principais
- Sistema de gamificação
- Fluxos de navegação
- Cofres financeiros
- Detecção de gastos recorrentes
- Perfis de agentes financeiros
- Experiência conversacional

---

## Prompt Utilizado

O desenvolvimento do projeto foi orientado por um prompt detalhado que descrevia o Saldoo como um Copiloto Financeiro Conversacional Gamificado.

O prompt incluiu requisitos como:

- Registro de receitas e despesas por linguagem natural
- Agentes financeiros inteligentes
- Sistema de níveis e XP
- Missões e conquistas
- Detecção de gastos recorrentes
- Gestão de metas através de Cofres Financeiros
- Interface inspirada em sistemas de progressão presentes em jogos de gerenciamento de recursos

Durante os testes também foi solicitado ao copiloto:

```text
Criar reserva viagem com meta de R$ 5.000
```

com o objetivo de validar a interpretação de metas financeiras por meio de linguagem natural.

---

## Reflexão Sobre o Processo

### O que funcionou bem

A utilização de Inteligência Artificial durante o planejamento e refinamento dos requisitos permitiu expandir significativamente a proposta inicial do projeto.

Foi possível identificar rapidamente novas funcionalidades, melhorar a experiência do usuário e estruturar um produto mais completo antes mesmo da implementação.

Além disso, a IA contribuiu para transformar um simples aplicativo de controle financeiro em uma plataforma com elementos de educação financeira e gamificação.

---

### O que não funcionou como esperado

Durante os testes foi solicitado ao assistente:

```text
Criar reserva viagem com meta de R$ 5.000
```

A expectativa era que o sistema identificasse automaticamente a intenção de criar uma nova meta financeira.

Entretanto, o comportamento observado indicou que o assistente estava preparado apenas para registrar gastos e receitas, solicitando informações sobre valores, categorias e despesas já realizadas.

Esse cenário demonstrou a importância de definir melhor os fluxos de intenção e o contexto das interações quando se trabalha com IA conversacional.

---

### O que aprendi sobre conversar com IAs

O principal aprendizado foi que a qualidade dos resultados está diretamente relacionada à qualidade das instruções fornecidas.

Durante a construção do projeto ficou evidente que:

- Prompts mais específicos geram resultados melhores.
- Refinamentos sucessivos melhoram significativamente a qualidade das respostas.
- A IA é extremamente eficiente para brainstorming e validação de ideias.
- Contexto é fundamental para reduzir ambiguidades.
- Testes em cenários reais ajudam a identificar limitações e oportunidades de melhoria.

---

## Objetivo

O Saldoo busca tornar a educação financeira mais acessível através da combinação entre Inteligência Artificial, experiência conversacional e gamificação, incentivando a construção de hábitos financeiros saudáveis de maneira simples e intuitiva.

---

## Próximos Passos

Algumas melhorias planejadas para futuras versões:

- Aprimorar a interpretação de metas financeiras por linguagem natural.
- Melhorar o fluxo conversacional do copiloto financeiro.
- Expandir os indicadores de saúde financeira.
- Melhorar a gestão de cofres e objetivos financeiros.
- Adicionar autenticação de usuários.
- Implementar histórico financeiro persistente.
- Evoluir as recomendações inteligentes geradas pela IA.
- Publicar novas versões com foco em experiência do usuário e acessibilidade.

---

## Considerações Finais

Este projeto representa um estudo prático sobre desenvolvimento assistido por Inteligência Artificial, UX conversacional e gamificação aplicada à educação financeira.

O objetivo principal não foi criar um produto finalizado, mas explorar novas formas de construção de software utilizando IA como parceira no processo de ideação, refinamento de requisitos e prototipação.
