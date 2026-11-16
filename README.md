# Porsche Sales Intelligence

Dashboard analítico de vendas de veículos Porsche, com filtros interativos e indicadores para apoiar decisões comerciais.

## Base de dados

- Arquivo tratado: `planilha_porsche_tratada.xlsx`
- Registros: base fictícia de vendas Porsche.
- Valores em US$.
- Data de referência: 15/11/2026.

### Tratamento aplicado

**Nomes dos vendedores**
- Padronização dos nomes dos vendedores para evitar duplicidades causadas por variações de grafia, espaços extras e capitalização.

**Datas inválidas**
- Registros com data inválida foram identificados e marcados como `INVALID`.
- Esses registros entram nos totais e nos filtros, mas ficam fora dos gráficos e dos KPIs que dependem de período.

## Filtros do dashboard

- Modelo Porsche
- Ano-modelo (Model Year)
- Cidade (City)
- Forma de pagamento (Pay method)
- Período

Todas as seções e indicadores reagem aos filtros ao mesmo tempo.

## Perguntas de negócio e KPIs

1. **Quais os principais modelos vendidos por cidade?**
   Heatmap de unidades por cidade e modelo, com ranking dos modelos líderes em cada cidade.

2. **Qual ano-modelo mais foi vendido em um período?**
   Unidades vendidas por ano-modelo, respeitando o filtro de período.

3. **Quais carros são populares em cada cidade?**
   Top 3 modelos por cidade, com volume de unidades e receita.

4. **Quanto da receita está travado em pedidos não entregues, e por quê?**
   Receita por status de entrega e cruzamento com a forma de pagamento.
   Pendente = todos os status exceto Delivered e Cancelled.

5. **Quais vendedores e estados concentram o melhor desempenho?**
   Ranking de vendedores e de estados por receita e quantidade de vendas.

6. **Como o preço se comporta com o ano-modelo e a quilometragem, e quais modelos geram mais receita?**
   Dispersão de preço e quilometragem por ano-modelo, preço médio por ano-modelo e ranking de modelos por receita.

## Indicadores principais

- Total de vendas e receita.
- Vendas entregues, pendentes, em trânsito e canceladas.
- Receita não entregue, que inclui pendências e pedidos em trânsito.

## Como usar

1. Abra o `index.html` no navegador.
2. Escolha os filtros no painel superior.
3. Use o botão **Limpar filtros** para voltar à visão completa.
4. Use **Imprimir / PDF** para gerar uma versão para impressão.



