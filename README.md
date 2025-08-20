# Cha.3TelecomX

Análise de Evasão de Clientes e Modelagem Preditiva
Este notebook contém uma análise exploratória dos dados de clientes de telecomunicações e a construção de modelos preditivos para identificar clientes com maior probabilidade de evasão (Churn).

Sumário
Extração de Dados: Carregamento do dataset.
Transformação de Dados: Pré-processamento dos dados, incluindo a remoção de colunas, codificação de variáveis categóricas (One-Hot Encoding) e avaliação de desequilíbrio de classes.
Correlação e Seleção de Variáveis: Análise da correlação entre variáveis numéricas e a variável alvo (Churn), e visualização das relações.
Modelagem Preditiva: Divisão dos dados em conjuntos de treino e teste, escalonamento de variáveis numéricas e treinamento de modelos de Regressão Logística e Random Forest.
Avaliação de Modelos: Avaliação do desempenho dos modelos utilizando métricas como Acurácia, Precision, Recall e F1-score.
Interpretações e Conclusões: Análise da importância das variáveis para cada modelo e interpretação dos resultados para propor estratégias de retenção.
Bibliotecas Utilizadas
pandas: Para manipulação e análise de dados.
numpy: Para operações numéricas.
matplotlib.pyplot: Para visualização de dados.
seaborn: Para visualização estatística de dados.
sklearn: Para pré-processamento, modelagem e avaliação de machine learning.
imblearn: Para lidar com dados desbalanceados (RandomUnderSampler, RandomOverSampler, SMOTE).
Como Executar o Notebook
Faça o upload do arquivo telecomx_treated_data.csv para o ambiente Google Colab.
Execute as células do notebook sequencialmente.
Análise e Resultados
O notebook realiza as seguintes etapas principais:

Carrega os dados e exibe as primeiras linhas.
Remove colunas consideradas menos relevantes para a análise.
Aplica One-Hot Encoding em variáveis categóricas.
Verifica o desequilíbrio da classe 'Churn' e demonstra o uso de técnicas de reamostragem (Undersampling e Oversampling).
Calcula e visualiza a matriz de correlação entre variáveis numéricas e Churn.
Gera boxplots para visualizar a relação entre 'customer.tenure', 'account.Charges.Total' e Churn.
Divide os dados em conjuntos de treino e teste.
Escalona as features numéricas utilizando StandardScaler.
Treina e avalia modelos de Regressão Logística e Random Forest.
Analisa a importância das variáveis para cada modelo e apresenta as 20 variáveis mais importantes em gráficos de barras.
Discute as métricas de desempenho dos modelos e compara seus resultados.
Propõe estratégias de retenção de clientes com base nos fatores que mais influenciam a evasão.
Conclusões Principais
A análise identificou que o tempo de contrato (customer.tenure), os encargos mensais (account.Charges.Monthly), os encargos totais (account.Charges.Total), o tipo de contrato (account.Contract_Two year), o serviço de internet (internet.InternetService_Fiber optic) e a utilização de serviços de segurança online (internet.OnlineSecurity_Yes) são os fatores que mais influenciam a evasão de clientes. A Regressão Logística apresentou um desempenho ligeiramente superior ao Random Forest na previsão de Churn.

Próximos Passos Sugeridos
Explorar técnicas de engenharia de features para criar novas variáveis relevantes.
Realizar uma seleção de features mais avançada.
Otimizar hiperparâmetros dos modelos existentes.
Experimentar outros algoritmos de classificação.
Implementar validação cruzada para uma avaliação mais robusta.
Este README fornece um resumo conciso do conteúdo e dos resultados do notebook, facilitando a compreensão do projeto e dos principais insights obtidos.

