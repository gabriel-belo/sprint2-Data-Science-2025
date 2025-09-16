# sprint2-Data-Science-2025

**Problema**: Baixa visibilidade no consumo real de insumos nas unidades de diagnóstico.

**Objetivo**: Prever a **quantidade de consumo mensal** com base em variáveis operacionais.

**Variável alvo**: `consumo_mensal`

**Variável preditora (simples)**: `numero_exames`


Para validar uma regressão linear, os seguintes pressupostos devem ser testados:

1. **Linearidade**: Relação linear entre preditores e variável alvo (verificado com scatter plot).
2. **Homoscedasticidade**: Resíduos com variância constante (plot resíduos vs. predição).
3. **Normalidade dos resíduos**: Verificado com histograma e teste de Shapiro-Wilk.
4. **Independência dos resíduos**: Importante em dados temporais (pode ser ignorado aqui).


O coeficiente angular (inclinação) indica o quanto o consumo aumenta a cada exame adicional realizado.

O intercepto indica o consumo estimado quando o número de exames é zero.

Aqui analisamos quais variáveis têm maior impacto no consumo.

- `numero_exames`: impacto direto
- `numero_funcionarios`: impacto operacional
- `dias_uteis`: influencia no tempo de operação

### Aplicação Prática:

Este modelo permite prever o consumo mensal de insumos com base em variáveis operacionais:

- **Benefícios**:
  - Melhor controle de estoque
  - Redução de perdas por falta ou excesso de materiais
  - Apoio ao planejamento logístico e compras

- **Limitações**:
  - Não considera eventos extraordinários
  - Depende da qualidade da entrada de dados
  - Não é adequado para mudanças abruptas sem re-treinamento

