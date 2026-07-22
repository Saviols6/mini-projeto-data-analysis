# Painel de Vendas — E-commerce Tech

Mini-projeto de análise de dados que transforma um pipeline em Python (Pandas, NumPy, Matplotlib) em um painel interativo, publicado como página estática.

**[🔗 Ver o painel ao vivo](https://saviols6.github.io/mini-projeto-data-analysis/)**

---

## 1. Definição do Problema de Negócio

### 1.1. O Problema de Negócio

Nossa loja de e-commerce está em fase de crescimento, registrando um volume cada vez maior de transações diárias. No entanto, essa grande quantidade de dados de vendas, em seu estado bruto, é como um baú de tesouro trancado: sabemos que há valor ali, mas não conseguimos acessá-lo.

Atualmente, muitas de nossas decisões estratégicas são baseadas em intuição e observações parciais, o que nos leva a enfrentar os seguintes desafios:

- **Gestão de Estoque Ineficiente**: não temos clareza sobre quais produtos são nossos "campeões de venda" e quais estão parados nas prateleiras. Isso resulta em excesso de estoque de itens de baixa procura e falta de produtos de alta demanda.
- **Marketing com Baixo Retorno**: nossas campanhas de marketing são genéricas, pois não sabemos quais categorias de produtos atraem mais os clientes ou em quais regiões geográficas nosso público está mais concentrado.
- **Perda de Oportunidades Sazonais**: não conseguimos identificar padrões ou tendências de vendas ao longo dos meses. Isso nos impede de planejar promoções estratégicas para períodos de alta ou de criar ações para impulsionar as vendas em meses de baixa.
- **Expansão sem Direção**: temos o desejo de expandir, mas não sabemos quais mercados regionais são mais promissores ou onde nossos esforços logísticos deveriam ser focados.

O problema central é a falta de visibilidade clara sobre a performance do negócio, o que nos impede de tomar decisões rápidas, inteligentes e baseadas em evidências.

### 1.2. Objetivos do Projeto

Este projeto de análise de dados visa transformar dados brutos de vendas em insights acionáveis, respondendo a quatro perguntas de negócio fundamentais:

| # | Pergunta | Objetivo |
|---|---|---|
| 01 | **O que vender?** | Identificar os produtos de maior sucesso para otimizar portfólio e estoque. |
| 02 | **Onde focar?** | Compreender quais categorias de produtos geram a maior parte da receita. |
| 03 | **Quando agir?** | Analisar a performance de vendas ao longo do tempo para identificar tendências, picos e sazonalidades. |
| 04 | **Para onde expandir?** | Mapear a distribuição geográfica das vendas para descobrir os mercados mais fortes. |

### 1.3. Solução Proposta

A solução consiste em consolidar, limpar e analisar o histórico de dados de vendas da plataforma. Utilizando ferramentas de análise de dados — Python com Pandas, NumPy e Matplotlib —, processamos essas informações e criamos um relatório visual que apresenta as descobertas de forma clara e intuitiva para as equipes de gestão, marketing e operações. O resultado final foi publicado como um painel HTML interativo (com Chart.js), para que qualquer pessoa possa explorar os dados sem precisar rodar código.

### 1.4. Resultados Esperados e Benefícios de Negócio

- **Otimização de Estoque**: com a lista dos produtos mais e menos vendidos, é possível ajustar compras, reduzir custos com armazenamento e evitar perda de vendas por falta de produto.
- **Marketing Direcionado e Eficaz**: sabendo quais categorias e regiões são mais lucrativas, a equipe de marketing pode criar campanhas segmentadas, aumentando o retorno sobre o investimento (ROI).
- **Planejamento Estratégico**: a visualização das tendências mensais permite melhor planejamento financeiro, promocional e de recursos, antecipando períodos de alta e baixa demanda.
- **Decisões Baseadas em Dados**: substitui a intuição por dados concretos, criando uma cultura orientada a dados que impulsiona o crescimento sustentável do negócio.

---

## O que o painel mostra

- KPIs gerais (faturamento total, ticket médio, pedidos, unidades vendidas).
- Top 10 produtos mais vendidos.
- Faturamento por categoria, por mês e por estado — respondendo diretamente às 4 perguntas de negócio.
- Filtros interativos por estado e categoria, recalculando tudo em tempo real.
- Curva de Pareto de concentração de clientes (quanto do faturamento vem de quantos clientes).
- Faturamento por status de entrega (Rápida x Normal), como leitura de cobertura logística.

## Sobre os dados

Os dados são **fictícios**, gerados por script (`sg_gera_dados_ficticios`) seguindo uma lógica controlada: 7 produtos, 8 cidades/estados, datas entre janeiro e abril de 2026, com desconto aleatório de até 10% para dois dos produtos. Servem para simular um cenário realista de análise, não representam vendas reais.

## Stack técnica

- **Análise original**: Python, Pandas, NumPy, Matplotlib, Seaborn (Jupyter Notebook).
- **Painel publicado**: HTML, CSS e JavaScript puro, com [Chart.js](https://www.chartjs.org/) para os gráficos interativos. Sem backend — os dados vêm embutidos no próprio arquivo.

## Como rodar localmente

Não precisa de servidor nem instalação. Basta abrir o arquivo `index.html` diretamente no navegador — os dados já estão embutidos no arquivo.

## Autor

**Sávio Giovani** — estudante de Engenharia de Controle e Automação (UPE).
