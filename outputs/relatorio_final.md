# Relatório Final — Análise das Lojas (Alura Store)

**Objetivo.** Identificar qual loja o Sr. João deve vender, com base em dados de faturamento, mix de categorias, satisfação dos clientes, giro de produtos e custo de frete.

**Bases e ferramentas.** CSVs consolidados, Pandas para ETL/KPIs e Matplotlib para visualizações. Todas as etapas foram executadas no notebook.

## Desenvolvimento da Análise

### 1) Faturamento Total por Loja
Comparamos o faturamento total (∑ preço × quantidade) por loja para identificar quem sustenta a receita da rede e quem performa abaixo da média.

### 2) Mix — Vendas por Categoria
Analisamos as categorias mais populares por loja para entender foco/composição do portfólio e possíveis lacunas.

### 3) Satisfação — Média de Avaliação por Loja
Avaliamos a nota média dos clientes (1 a 5) para mensurar percepção de qualidade/serviço.

### 4) Giro — Produtos Mais e Menos Vendidos
Levantamos os campeões de venda (pulmão do faturamento) e os itens de baixa rotação (candidatos a revisão).

### 5) Logística — Frete Médio por Loja
Comparamos o custo médio de frete por loja (pago pelo cliente), métrica que impacta conversão e satisfação.

## KPIs Consolidados

| loja   | Faturamento_Total   |   Media_Avaliacao | Frete_Medio   |   Ineficiência |
|:-------|:--------------------|------------------:|:--------------|---------------:|
| loja_4 | R$ 1,384,497.58     |              4    | R$ 31.28      |          0.72  |
| loja_1 | R$ 1,534,509.12     |              3.98 | R$ 34.69      |          0.5   |
| loja_3 | R$ 1,464,025.03     |              4.05 | R$ 33.07      |          0.34  |
| loja_2 | R$ 1,488,459.06     |              4.04 | R$ 33.62      |          0.337 |

## Detalhes por Loja

### loja_4
    - **Faturamento:** R$ 1,384,497.58
    - **Avaliação média:** 4.00
    - **Frete médio:** R$ 31.28
    - **Top categorias:**  
    - moveis (480 vendas)
- eletronicos (451 vendas)
- brinquedos (338 vendas)
    - **Top produtos:**  
    - Cama box (62 vendas)
- Faqueiro (59 vendas)
- Cama king (56 vendas)
    - **Produtos com menor giro:**  
    - Guitarra (33 vendas)
- Guarda roupas (34 vendas)
- Violão (37 vendas)

### loja_1
    - **Faturamento:** R$ 1,534,509.12
    - **Avaliação média:** 3.98
    - **Frete médio:** R$ 34.69
    - **Top categorias:**  
    - moveis (465 vendas)
- eletronicos (448 vendas)
- brinquedos (324 vendas)
    - **Top produtos:**  
    - Guarda roupas (60 vendas)
- Micro-ondas (60 vendas)
- TV Led UHD 4K (60 vendas)
    - **Produtos com menor giro:**  
    - Celular ABXY (33 vendas)
- Headset (33 vendas)
- Panela de pressão (35 vendas)

### loja_3
    - **Faturamento:** R$ 1,464,025.03
    - **Avaliação média:** 4.05
    - **Frete médio:** R$ 33.07
    - **Top categorias:**  
    - moveis (499 vendas)
- eletronicos (451 vendas)
- brinquedos (315 vendas)
    - **Top produtos:**  
    - Kit banquetas (57 vendas)
- Cama king (56 vendas)
- Mesa de jantar (56 vendas)
    - **Produtos com menor giro:**  
    - Blocos de montar (35 vendas)
- Jogo de copos (36 vendas)
- Micro-ondas (36 vendas)

### loja_2
    - **Faturamento:** R$ 1,488,459.06
    - **Avaliação média:** 4.04
    - **Frete médio:** R$ 33.62
    - **Top categorias:**  
    - moveis (442 vendas)
- eletronicos (422 vendas)
- brinquedos (313 vendas)
    - **Top produtos:**  
    - Iniciando em programação (65 vendas)
- Micro-ondas (62 vendas)
- Bateria (61 vendas)
    - **Produtos com menor giro:**  
    - Jogo de tabuleiro (32 vendas)
- Impressora (34 vendas)
- Mesa de jantar (34 vendas)

## Conclusão e Recomendação

**Loja recomendada para venda:** **loja_4**

**Motivos (baseados nos dados):**
- Menor desempenho relativo no composto de métricas (**índice de ineficiência** mais alto).
- Faturamento abaixo dos pares e/ou concentração excessiva de portfólio.
- Avaliação média inferior e/ou frete médio superior, impactando conversão e percepção.
- Maior presença de itens de baixa rotação.

**Observação:** os pesos do índice (faturamento=0.5, avaliação=0.3, frete=0.2) podem ser ajustados conforme a estratégia (ex.: priorizar experiência do cliente ou logística).