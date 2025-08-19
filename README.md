# Projeto Telecom X – Análise de Evasão de Clientes (Churn)

## Descrição do Projeto
Este projeto tem como objetivo analisar e prever a evasão de clientes (Churn) de uma empresa de telecomunicações. Foram utilizados dados tratados, transformações de variáveis categóricas, análise exploratória, balanceamento de classes, normalização de dados e criação de modelos preditivos.  

Os modelos utilizados foram:
- **Regressão Logística** (necessita de normalização)  
- **Random Forest** (não necessita de normalização)  

Além disso, o projeto identifica as variáveis mais relevantes que influenciam a evasão e propõe estratégias de retenção de clientes com base nos resultados obtidos.

---

## Estrutura do Repositório
- `Telecom_X_Projeto.ipynb` – Notebook com todo o código, análises, visualizações e modelagem.  
- `dados_tratados.csv` – Arquivo CSV com os dados limpos e tratados utilizados no projeto.  

---

## Etapas do Projeto
1. **Carregamento dos Dados** – Importação do CSV com os dados tratados.  
2. **Pré-processamento** – Remoção de colunas irrelevantes, tratamento de variáveis categóricas (One-Hot Encoding) e análise de proporção de classes.  
3. **Balanceamento de Classes** – Aplicação de SMOTE para equilibrar a proporção entre clientes que evadiram e clientes ativos.  
4. **Normalização** – Escalonamento de dados para modelos que dependem de distância (como Regressão Logística).  
5. **Análise Exploratória** – Visualização de correlações, boxplots e scatter plots para investigar padrões de evasão.  
6. **Divisão Treino/Teste** – Separação dos dados em conjuntos de treino (80%) e teste (20%).  
7. **Modelagem Preditiva** – Treinamento de Regressão Logística e Random Forest.  
8. **Avaliação de Modelos** – Métricas utilizadas: Acurácia, Precisão, Recall, F1-score e Matriz de Confusão.  
9. **Análise de Variáveis** – Identificação das features mais relevantes para cada modelo.  
10. **Conclusões e Estratégias de Retenção** – Principais insights e recomendações práticas para reduzir evasão de clientes.  

---

## Principais Fatores de Evasão Identificados
- **Tempo de contrato**: Clientes com menor tempo de serviço apresentam maior probabilidade de evasão.  
- **Tipo de serviço de internet**: Fibra óptica está associada a maior evasão; ausência de serviço de internet, menor.  
- **Encargos mensais e totais**: Valores mais altos impactam a probabilidade de evasão.  
- **Método de pagamento**: Cheque eletrônico correlaciona-se com maior evasão.  
- **Tipo de contrato**: Contratos de longo prazo (1 ou 2 anos) reduzem a probabilidade de evasão.  
- **Serviços adicionais**: Ausência de serviços como segurança online, suporte técnico, backup online e proteção de dispositivo aumenta a evasão.  
- **Cidadão sênior**: Clientes idosos têm leve aumento na probabilidade de evasão.  
- **Contas diárias**: Reflete a carga financeira percebida pelo cliente e impacta na evasão.  

---

## Estratégias de Retenção Propostas
- Foco em clientes de curto prazo com programas de engajamento e incentivos.  
- Melhoria e monitoramento do serviço de Fibra Óptica.  
- Otimização de preços e pacotes de serviços.  
- Incentivo a contratos de longo prazo.  
- Promoção de serviços adicionais com demonstrações ou testes gratuitos.  
- Revisão do método de pagamento por cheque eletrônico.  
- Programas específicos para cidadãos seniores.  
- Monitoramento de “Contas Diárias” como indicador precoce de risco.  

---

## Tecnologias e Bibliotecas Utilizadas
- Python  
- Pandas, NumPy  
- Scikit-learn (Logistic Regression, Random Forest, metrics)  
- Imbalanced-learn (SMOTE)  
- Seaborn, Matplotlib  

---

## Autor
Felipe Diego
