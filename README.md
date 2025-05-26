# Descrição Técnica da Planilha de Simulação de Investimentos
Esta planilha Excel foi desenvolvida para auxiliar no controle e simulação de investimentos, permitindo comparar diferentes estratégias de alocação de ativos (Conservadora, Moderada e Agressiva) e analisar seus desempenhos ao longo do tempo. A planilha é composta por duas abas principais: Carteiras e Dados.

# Funcionalidades Principais

## 1. Aba "Carteiras"
Alocação de Ativos: Permite definir os percentuais de investimento em diferentes ativos (DÓLAR, CDI, IVVB11, BOVA11, SMAL11) para três perfis de risco:

Conservador: Foco em segurança, com maior peso em CDI (90%) e menor exposição a ativos voláteis.

Moderado: Equilíbrio entre risco e retorno, com distribuição mais diversificada (50% CDI, 15% em outros ativos).

Agressivo: Maior exposição a ativos de maior risco e potencial retorno (30% em IVVB11 e SMAL11).

Indicadores: Exibe métricas como retorno total, retorno médio, risco (volatilidade) e índice Sharpe para cada carteira, calculados com base nos dados históricos.

Fórmulas Destacadas:

SUMPRODUCT: Usada para calcular o retorno das carteiras com base nos pesos definidos.

IFERROR + INDEX/MATCH: Recupera os percentuais de alocação para exibição consolidada.

# 2. Aba "Dados"
Contém dados históricos mensais de retorno dos ativos (de 2016 a 2021) e cálculos estatísticos avançados:

Retorno Ano a Ano: Calcula o retorno anualizado para cada ativo e carteira.

Estatísticas:

Retorno Total: Soma dos retornos acumulados.

Retorno Médio: Média dos retornos mensais anualizada.

Risco (Volatilidade): Desvio padrão dos retornos mensais ajustado para anual.

Índice Sharpe: Mede o retorno ajustado ao risco (quanto maior, melhor).

Evolução de 100: Simula o crescimento de um investimento inicial de 100 unidades ao longo do tempo.

Retorno e Risco em 12 meses: Análise móvel para avaliar desempenho e volatilidade em janelas de um ano.

# Insights Extraídos da Planilha

1. Comparação entre Perfis de Risco
Carteira Conservadora:

Menor volatilidade (risco), mas retornos mais modestos.

Ideal para investidores avessos a risco ou com objetivos de curto prazo.

Carteira Agressiva:

Maior potencial de retorno, especialmente em períodos de alta dos mercados (ex.: IVVB11 e SMAL11 tiveram retornos significativos em 2020).

Volatilidade elevada, podendo apresentar perdas acentuadas em crises (ex.: março de 2020).

![comparação entre perfis](https://github.com/user-attachments/assets/dc8037fa-0488-4437-8027-f78ed71cb82a)

2. Desempenho dos Ativos
CDI: Retorno estável e previsível, porém limitado.

IVVB11 (ETF S&P 500): Boa performance em períodos de alta do mercado internacional, mas sensível a crises globais.

BOVA11 e SMAL11 (ETFs de ações brasileiras): Maior volatilidade, com potencial de retorno em ciclos de alta da bolsa.

3. Análise de Risco-Retorno
O Índice Sharpe ajuda a identificar qual carteira oferece o melhor retorno por unidade de risco. Por exemplo:

![Análise d riico retorno](https://github.com/user-attachments/assets/7e4ea6c1-3862-4831-9add-2823a3e245f9)

Se a carteira Moderada tem um Sharpe maior que a Agressiva, pode ser mais eficiente em termos de risco/retorno.

![Indic Sharpe](https://github.com/user-attachments/assets/79fb2629-c381-4884-8efa-35728265a36b)

4. Evolução Temporal
A aba "Dados" permite visualizar como cada ativo e carteira se comportou em diferentes cenários (ex.: crise de 2020, recuperação em 2021).

A simulação "Evolução de 100" mostra o crescimento hipotético de um investimento ao longo do tempo.

# Como Utilizar a Planilha

Edite os pesos: Na aba "Carteiras", ajuste os percentuais nos campos amarelos para simular diferentes estratégias.

Analise os resultados: Verifique os indicadores (retorno, risco, Sharpe) para comparar as carteiras.

Explore os dados históricos: Use a aba "Dados" para entender o comportamento dos ativos em diferentes períodos.

Tome decisões: Baseie suas escolhas de alocação nos insights gerados, considerando seu perfil de risco e objetivos.

# Observações Técnicas

Fórmulas Avançadas: A planilha utiliza funções como SUMPRODUCT, STDEV, AVERAGE e cálculos anualizados para garantir precisão.

Atualização: Para manter a análise relevante, os dados históricos podem ser atualizados periodicamente.

Flexibilidade: A estrutura permite adicionar novos ativos ou ajustar os perfis de carteira conforme necessário.

Esta planilha é uma ferramenta poderosa para quem deseja simular estratégias de investimento e tomar decisões mais informadas. Clone o repositório, explore os dados e adapte-os às suas necessidades!
