# 📊 Projeto — Predição de Churn Bancário com Árvore de Decisão
<img width="800" height="800" alt="image" src="https://github.com/user-attachments/assets/49b5f646-8544-4885-8196-77000f88aa5b" />

Comparação entre uma Árvore de Decisão completa e uma versão simplificada para prever a evasão (churn) de clientes bancários, avaliando o impacto da redução de variáveis no desempenho do modelo.

## 📌 Sobre o Projeto

Este projeto aplica técnicas de Ciência de Dados e Machine Learning para prever a evasão de clientes (churn) em uma instituição financeira utilizando o algoritmo de Árvore de Decisão.

O trabalho dá continuidade às etapas anteriores do projeto, nas quais foram realizados o tratamento dos dados, a codificação das variáveis categóricas, o balanceamento das classes e a aplicação do algoritmo Naive Bayes. Nesta etapa, são construídos e comparados dois modelos de Árvore de Decisão: um modelo completo e outro reduzido, utilizando apenas as variáveis mais relevantes para a previsão.

## 🎯 Problema de Negócio / Pergunta de Pesquisa

*Problema:* Identificar clientes com maior probabilidade de cancelar seus serviços bancários para permitir ações preventivas de retenção.

*Objetivo:* Construir e comparar modelos de Árvore de Decisão para prever o churn de clientes, analisando o impacto da simplificação do modelo sobre a acurácia e a capacidade de identificar clientes propensos ao cancelamento.

*Público / Impacto:*

- equipes de CRM;
  
- times de retenção de clientes;
  
- analistas de risco;
  
- gestores de relacionamento.

Um modelo eficiente permite identificar clientes em risco antes do cancelamento, reduzindo perdas financeiras e aumentando a fidelização.

## 📊 Fonte de Dados

*Variáveis principais:*

- idade;

- renda;
  
- histórico de pagamentos;
  
- tempo de relacionamento com o banco;
  
- demais atributos cadastrais e financeiros utilizados para prever churn.

#### Além disso, a análise de importância das variáveis mostra que apenas as duas características mais relevantes foram utilizadas na versão reduzida da árvore.

Pré-processamento realizado

Foi possível identificar que anteriormente foram executadas as seguintes etapas:

tratamento de valores ausentes;
transformação de variáveis categóricas;
balanceamento das classes;
análise exploratória;
divisão entre treino e teste.

Essas etapas já haviam sido realizadas antes da construção da árvore de decisão.

## 🛠 Tecnologias Utilizadas

*Python:*

- pandas

- numpy

- matplotlib
  
- seaborn
  
- scikit-learn

*Modelos:*

- DecisionTreeClassifier

- Naive Bayes (comparação com projeto anterior)

*Métricas:*

- Accuracy

- Precision

- Recall

- F1-score

- Matriz de Confusão

*Ambiente:* Jupyter Notebook

## 🔍 Metodologia
*Coleta dos dados:* Utilização da base de clientes bancários preparada nos módulos anteriores.

*Limpeza e tratamento:* Como o foco deste módulo é a modelagem, a base já estava previamente tratada:

- tratamento de valores faltantes;

- transformação de variáveis categóricas;

- balanceamento das classes;

- separação entre treino e teste.

## Modelagem

*Foram treinados dois modelos:*

- Árvore de Decisão completa utilizando todas as variáveis;

- Árvore de Decisão reduzida utilizando apenas as variáveis mais importantes.

O critério de divisão adotado foi Gini.

## Avaliação

*Os modelos foram avaliados por meio de:*

- Accuracy;

- Precision;

- Recall;

- F1-score;

- Matriz de Confusão;

- Importância das variáveis.

Também foi realizada a visualização da estrutura da árvore e da importância das features.

## 📈 Resultados e Métricas
- Modelo 1 — Árvore Completa
Métrica  | Valor

Accuracy  |  0,792

Precision (macro)  | 0,690

Recall (macro)  | 0,710

F1-score  | 0,700

- Modelo 2 — Árvore Reduzida
Métrica  | Valor

Accuracy  | 0,850

Precision (macro)  | 0,780

Recall (macro)  | 0,730

F1-score  | 0,750

### Comparação com Naive Bayes

#### *O notebook também compara os resultados obtidos anteriormente com Naive Bayes:*

Modelo | Accuracy | Teste	Recall | Teste

Naive Bayes | 0,555 | 0,648

Árvore Completa | 0,792	superior ao Naive Bayes

Árvore Reduzida | 0,850	desempenho mais equilibrado

### *Modelo final escolhido:*

A Árvore de Decisão reduzida apresentou melhor desempenho geral, alcançando maior acurácia e aumento significativo da precisão em relação ao modelo completo, demonstrando que a simplificação da árvore contribuiu para uma melhor capacidade de generalização.

## 💡 Principais Insights e Implicações
A Árvore de Decisão apresentou desempenho significativamente superior ao Naive Bayes na previsão de churn.

A redução da árvore utilizando apenas as variáveis mais importantes aumentou a acurácia de 79,2% para 85,0%, mostrando que modelos mais simples podem generalizar melhor.

Embora o recall da classe de churn tenha sofrido pequena redução, houve aumento expressivo na precisão, reduzindo falsos positivos.

A análise de importância das variáveis permitiu identificar quais atributos exercem maior influência sobre a decisão do modelo, tornando-o mais interpretável para o negócio.
Implicação prática

### Uma Árvore de Decisão é uma ferramenta interessante para problemas de churn por combinar boa capacidade preditiva com alta interpretabilidade. Além de identificar clientes com maior risco de evasão, o modelo permite compreender quais fatores mais influenciam essa decisão, facilitando o planejamento de ações de retenção.

## 👩‍💻 Sobre a Autora

Desenvolvido por Marina Napoleão — Cientista de Dados / Analista de Dados. 
### LinkedIn <https://www.linkedin.com/in/marina-napoleao/>
### GitHub <https://github.com/marinanapoleao> 
