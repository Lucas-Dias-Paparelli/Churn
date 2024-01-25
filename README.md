Português:
# Projeto: Previsão de Churn de Clientes

## Visão Geral:
Este projeto concentra-se na previsão de churn de clientes usando técnicas de aprendizado de máquina. O conjunto de dados foi inicialmente importado usando a biblioteca pandas, permitindo manipulação e pré-processamento dos dados. Vários passos foram realizados para preparar os dados para algoritmos de aprendizado de máquina.

## Pré-processamento de Dados:
1. **Seleção de Colunas:**
   - As colunas 'Surname', 'RowNumber' e 'CustomerId' foram identificadas como irrelevantes para o algoritmo de aprendizado de máquina e foram removidas durante o pré-processamento dos dados.

2. **Codificação de Geografia:**
   - A coluna 'Geography', contendo os países 'France', 'Spain' e 'Germany', foi transformada em três colunas binárias usando a função `get_dummies`. Cada coluna binária representava se a entrada pertencia a um país específico (1) ou não (0).

3. **Codificação de Gênero:**
   - A coluna 'Gender', inicialmente contendo 'Female' e 'Male', foi convertida em valores binários, onde 'Female' foi representado como 1 e 'Male' como 0 para uma melhor compreensão do algoritmo.

4. **Normalização:**
   - Como o algoritmo LinearSVC não é adequado para dados desbalanceados, o conjunto de dados foi normalizado e balanceado para melhorar seu desempenho. Essa etapa contribuiu para alcançar resultados mais satisfatórios.

5. **Remoção de Dados:**
   - Após o pré-processamento dos dados, a coluna 'Geography' foi removida, pois não era mais necessária.

## Modelos de Aprendizado de Máquina:
Três modelos de aprendizado de máquina foram utilizados para prever o churn de clientes:

1. **LinearSVC:**
   - Apesar de apresentar resultados melhorados após a normalização e balanceamento dos dados, o LinearSVC não superou outros modelos no tratamento de dados desbalanceados.

2. **Árvore de Decisão:**
   - O modelo de Árvore de Decisão foi introduzido, pois tende a lidar bem com dados desbalanceados.

3. **Random Forest:**
   - Random Forest destacou-se como o algoritmo mais eficaz para este caso, demonstrando maior acurácia e equilíbrio entre precisão e recall.

## Conclusão:
Em conclusão, o modelo Random Forest mostrou-se o mais adequado para prever o churn de clientes neste cenário. Os passos de pré-processamento, incluindo normalização e balanceamento de dados, contribuíram significativamente para o desempenho do modelo. O processo detalhado descrito acima garante uma compreensão abrangente das etapas de pré-processamento de dados e seleção de modelo.

## Contribuições e Feedback

Se você deseja contribuir ou fornecer feedback, fique à vontade para abrir issues ou pull requests. Sua participação é bem-vinda!

----------------------------------------------------------------------------------------------------------------------

English:
# Project: Customer Churn Prediction

## Overview:
This project focuses on predicting customer churn using machine learning techniques. The dataset was initially imported using the pandas library, allowing for data manipulation and preprocessing. Several steps were taken to prepare the data for machine learning algorithms.

## Data Preprocessing:
1. **Column Selection:**
   - The 'Surname', 'RowNumber', and 'CustomerId' columns were identified as irrelevant for the machine learning algorithm and were removed during data preprocessing.

2. **Geography Encoding:**
   - The 'Geography' column, containing countries 'France', 'Spain', and 'Germany', was transformed into three binary columns using the `get_dummies` function. Each binary column represented whether the entry belonged to a specific country (1) or not (0).

3. **Gender Encoding:**
   - The 'Gender' column, initially containing 'Female' and 'Male', was converted into binary values, where 'Female' was represented as 1, and 'Male' as 0 for better algorithm comprehension.

4. **Normalization:**
   - As the LinearSVC algorithm is not suitable for imbalanced data, the dataset was normalized and balanced to improve its performance. This step contributed to achieving better results.

5. **Data Removal:**
   - After data preprocessing, the 'Geography' column was removed as it was no longer needed.

## Machine Learning Models:
Three machine learning models were employed to predict customer churn:

1. **LinearSVC:**
   - Despite achieving improved results after normalizing and balancing the data, LinearSVC did not outperform other models in handling imbalanced data.

2. **Decision Tree:**
   - The Decision Tree model was introduced as it tends to handle imbalanced data well.

3. **Random Forest:**
   - Random Forest emerged as the most effective algorithm for this case, demonstrating higher accuracy and balance between precision and recall.

## Conclusion:
In conclusion, the Random Forest model proved to be the most suitable for predicting customer churn in this scenario. The preprocessing steps, including data normalization and balancing, significantly contributed to model performance. The detailed process outlined above ensures a comprehensive understanding of the data preprocessing and model selection steps.

##Contributions and Feedback

If you wish to contribute or provide feedback, feel free to open issues or pull requests. Your participation is welcomed!
