# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)



## 🎯 Objetivos Deste Desafio de Projeto (Lab)



## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   Se carregó o arquivo 'dataset-1000-com-preco-promocional-e-renovacao-estoque.csv' da pasta 'datasets' deste repositório. Para treinar e testar o modelo de previsão de estoque de ML.

### 2. Construir/Treinar

-   No SageMaker Canvas, se fez a importação do dataset selecionado.
-   Configurando as variáveis de entrada e saída de acordo com os dados.
-   Se iniciou o treinamento do modelo. Apresentando o seguinte resultado:
  
    <img src="/Images/ModelStatus.png" alt="Resultado Canvas - anâlise arquivo do dataset">

### 3. Analisar

-   As métricas de performance do modelo preditor da amazon, para o dataset escolhido, foram:
    
        Promedio Weighted Quantile Loss (Avg. wQL) = 0.138
        Mean Absolute Percentage Error (MAPE) = 0.212
        Weighted Absolute Percentage Error (WAPE) = 0.187
        Root Mean Square Error (RMSE) = 20.364
        Mean Absolute Scaled Error (MASE) = 0.000

    Sendo as datas dos feriados no Brasil a coluna de aumento da precisão no modelo preditor com o 82.88% e
    as colunas de preço e promoções as que diminuem com 9.78% e 7.34%.
    Este relatório contém análise de modelo para o candidato Canvas1721864095976-trial-me. O modelo usado é
    um modelo de previsão de séries temporais treinado cujo objetivo é minimizar a métrica de qualidade
    "Perda de quantil ponderada média".

### 4. Prever

-   O modelo treinado para fazer previsões de estoque por 9 días do produto "1000" é o seguinte:
    <img src="/Images/single_prediction_9.png" alt="Resultado Canvas - anâlise produto 1000 do dataset para 9 dias">
-   O modelo treinado para fazer previsões de estoque por 1 día do produto "1000" é o seguinte:
    <img src="/Images/single_prediction_1.png" alt="Resultado Canvas - anâlise produto 1000 do dataset">
    
A conclusão individual para o produto "1000" indica que na previsão de 9 días o preditor se asemelha mais ao comportamento real de estoque do produto.

<img src="/Images/DadosProduto1000.png" alt="Comportamento Produto 1000">







