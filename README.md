📡 Prevendo Churn de Clientes com Machine Learning
Visão Geral do Projeto
Este projeto apresenta um pipeline completo de Machine Learning para prever a evasão de clientes (churn) em uma empresa de telecomunicações fictícia, a Telecom X. Partindo de uma análise exploratória inicial, o projeto evolui para a construção, avaliação e interpretação de modelos preditivos, culminando em recomendações estratégicas para o negócio.

Este foi o desafio final da formação em ETL da Turma G8 do programa ONE (Oracle Next Education).

🎯 O Desafio de Negócio
A alta taxa de churn é um dos problemas mais críticos para empresas de serviço por assinatura. Perder um cliente custa muito mais do que adquirir um novo. O desafio central deste projeto foi responder à seguinte pergunta:

É possível, com base nos dados históricos, prever quais clientes têm maior probabilidade de cancelar seus serviços e quais fatores mais influenciam essa decisão?

🛠️ Tecnologias e Bibliotecas Utilizadas
Linguagem: Python 3.11

Manipulação e Análise: Pandas, NumPy

Visualização de Dados: Plotly, Matplotlib, Seaborn

Machine Learning: Scikit-learn, Imbalanced-learn (para SMOTE)

Ambiente: Google Colab / Jupyter Notebook

🔄 Pipeline do Projeto
O projeto foi estruturado em um fluxo de trabalho completo, da análise à predição:

Fase 1: Análise Exploratória de Dados (EDA)
Investigação inicial para entender a distribuição dos dados e a taxa geral de churn.

Criação de visualizações interativas para identificar padrões visuais entre variáveis categóricas/numéricas e a evasão de clientes.

Fase 2: Pré-processamento e Engenharia de Features
Limpeza dos Dados: Remoção de colunas irrelevantes e tratamento de valores ausentes (NaN) através de imputação (mediana).

Encoding: Conversão de variáveis categóricas em formato numérico utilizando One-Hot Encoding (get_dummies).

Padronização: Aplicação de StandardScaler nas variáveis numéricas para normalizar suas escalas, otimizando o desempenho de modelos lineares.

Balanceamento de Classes: Utilização da técnica SMOTE no conjunto de treino para corrigir o desbalanceamento entre clientes que evadiram e os que não evadiram.

Fase 3: Modelagem e Treinamento
Foram treinados e comparados dois modelos de classificação com abordagens distintas:

Regressão Logística: Como um modelo de baseline, rápido e interpretável.

Random Forest: Como um modelo mais robusto e de alto desempenho, baseado em ensemble de árvores de decisão.

Fase 4: Avaliação e Interpretação
Os modelos foram avaliados com base em métricas de negócio relevantes para o problema de churn, como Recall, Precision e F1-Score, além da Matriz de Confusão.

O Random Forest foi selecionado como o modelo final devido ao seu desempenho superior e equilíbrio entre as métricas.

Foi realizada uma análise de Feature Importance para identificar os principais fatores preditivos.

📊 Principais Resultados e Insights
Desempenho do Modelo Final (Random Forest): O modelo foi capaz de prever corretamente ~78% dos clientes que realmente iriam cancelar o serviço (Recall), com uma precisão de ~60%, mostrando-se uma ferramenta eficaz para direcionar ações de retenção.

Fatores Mais Influentes no Churn: A análise de importância das variáveis revelou que os principais impulsionadores da evasão são:

Tipo de Contrato: Ser Month-to-month (mensal) é o fator de maior peso.

Tempo de Contrato (Tenure): Clientes com poucos meses de casa têm altíssima probabilidade de sair.

Faturamento Mensal (MonthlyCharges): Faturas mais altas estão associadas a um maior risco de churn.

💡 Recomendações Estratégicas
Com base nos insights, foram propostas as seguintes ações para a Telecom X:

Focar em Contratos de Longa Duração: Criar campanhas para migrar clientes de planos mensais para anuais.

Programa de Retenção para Novos Clientes: Implementar um acompanhamento proativo nos primeiros 3-6 meses.

Incentivar Pagamentos Automáticos: Oferecer descontos para quem sair do boleto eletrônico, reduzindo o atrito.

Desenvolvido com 🧠 por Miguel Antônio Barbosa Caetano

📧 miguelantoniobsk@gmail.com | 💼 www.linkedin.com/in/miguel-antoniobc
