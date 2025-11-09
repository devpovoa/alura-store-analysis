# 🏪 Alura Store — Análise de Desempenho das Lojas

## 📋 Descrição do Projeto
Este projeto foi desenvolvido como parte do **Desafio do Alura Challenger**, com o objetivo de auxiliar o **Sr. João**, proprietário da rede fictícia **Alura Store**, a decidir **qual loja deve ser vendida** com base em dados reais de desempenho.

A análise envolveu dados de **vendas, categorias, avaliações, produtos e frete**, fornecidos em arquivos CSV de quatro lojas diferentes.  
A partir desses dados, foram geradas **métricas, visualizações e um relatório automatizado**, culminando na recomendação final:  
> 🔎 **A Loja 4 é a candidata ideal para ser vendida**, devido ao menor desempenho global.

---

## 🧠 Objetivo da Análise
> Identificar, com base em dados quantitativos e qualitativos, qual loja apresenta menor eficiência operacional e comercial.

Para isso, foram analisados os seguintes aspectos:

- 💰 **Faturamento total por loja**  
- 🏷️ **Categorias de produtos mais vendidas**  
- ⭐ **Avaliação média dos clientes**  
- 📦 **Produtos mais e menos vendidos**  
- 🚚 **Frete médio por loja (custo pago pelo cliente)**  
- 🌍 *(Extra)* **Distribuição geográfica das vendas**

---

## 🧰 Ferramentas e Tecnologias Utilizadas

| Categoria | Tecnologias |
|------------|-------------|
| **Linguagem** | Python 3.12+ |
| **Ambiente** | Jupyter Notebook / Google Colab |
| **Análise de Dados** | `pandas`, `numpy` |
| **Visualização** | `matplotlib`, `seaborn` |
| **Relatório Dinâmico** | Markdown automático via `Python` |
| **Extra (opcional)** | `folium` — mapa interativo de vendas |
| **Controle de Versão** | Git (commit semântico) |

---

## 🔍 Etapas da Análise

### 1️⃣ Leitura e Tratamento dos Dados
- Carregamento automático dos 4 arquivos CSV (`database/loja_X.csv`).  
- Padronização de colunas (`preço → preco`, `avaliação_da_compra → avaliacao`, etc.).  
- Criação de colunas derivadas (`receita`, `quantidade`, etc.).  
- Consolidação de todas as lojas em um único DataFrame.

### 2️⃣ Faturamento Total por Loja
- Cálculo do faturamento total (∑ preço × quantidade).  
- Gráfico de barras verticais mostrando o desempenho de cada loja.

### 3️⃣ Vendas por Categoria
- Agrupamento por `categoria` e contagem de vendas.  
- Gráfico de barras horizontais com as categorias mais populares.

### 4️⃣ Média de Avaliação por Loja
- Cálculo da média das notas dos clientes (1 a 5).  
- Gráfico de barras com destaque para lojas mais e menos bem avaliadas.

### 5️⃣ Produtos Mais e Menos Vendidos
- Identificação dos produtos com maior e menor giro de vendas.  
- Visualização das Top 10 vendas gerais e dos produtos encalhados.

### 6️⃣ Frete Médio por Loja
- Cálculo do custo médio de frete por loja.  
- Gráfico comparativo evidenciando o impacto logístico nas vendas.

### 7️⃣ Extra: Análise Geográfica
- Uso de colunas `lat` e `lon` para mapear a distribuição das vendas.  
- Visualização em **gráfico de dispersão** ou **mapa interativo (Folium)**.

### 8️⃣ Relatório Final Automático
- Geração de relatório dinâmico em `outputs/relatorio_final.md`.  
- Inclui KPIs, top categorias/produtos e recomendação automática.

---

## 📊 Principais Resultados

| Loja | Faturamento | Avaliação Média | Frete Médio | Desempenho |
|------|--------------|-----------------|--------------|-------------|
| Loja 1 | Alto | Boa | Baixo | ✅ Eficiente |
| Loja 2 | Médio | Boa | Médio | ✅ Eficiente |
| Loja 3 | Alto | Regular | Médio | ⚙️ Estável |
| **Loja 4** | **Baixo** | **Baixa** | **Alto** | ❌ Ineficiente |

📈 **Conclusão:**  
> A **Loja 4** apresentou o **menor faturamento**, **piores avaliações** e o **frete mais caro** entre todas as lojas.  
> Esses fatores combinados indicam **ineficiência operacional** e **baixa atratividade comercial**, tornando-a a candidata mais adequada para venda.

---

## 📁 Estrutura de Pastas

alura_store_challenge/
│
├── database/ # CSVs de cada loja (dados brutos)
├── outputs/ # Imagens, mapas e relatório final
├── notebooks/ # (opcional) versões intermediárias
├── README.md # Este arquivo
└── requirements.txt # Dependências do projeto

---

## 🧾 Relatório Gerado
O relatório dinâmico (`outputs/relatorio_final.md`) contém:
- Introdução, desenvolvimento e conclusão;
- Tabelas com KPIs consolidados;
- Top categorias e produtos por loja;
- Recomendação automática da loja a ser vendida.

---

## 🧱 Commit e Versionamento

> Commit principal usado para consolidar o projeto:


---

## 💡 Aprendizados Técnicos

- Manipulação e consolidação de dados com **Pandas**.  
- Criação de gráficos customizados com **Matplotlib** e **Seaborn**.  
- Boas práticas de limpeza e normalização de dados.  
- Geração de relatórios dinâmicos e automatizados.  
- Aplicação de raciocínio analítico e **storytelling de dados**.

---

## 🏁 Resultado Final

> 💼 **Conclusão:**  
> Após todas as análises, a **Loja 4** apresentou o **pior desempenho geral** em faturamento, avaliação e custo logístico.  
> Assim, recomenda-se sua **venda estratégica**, concentrando investimentos nas demais lojas para maximizar o retorno do Sr. João.

---

