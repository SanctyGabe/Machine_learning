# 🍎🍅 Classificação de Imagens -- Apples vs Tomatoes

## 📌 Sobre o projeto

Este projeto treina uma **rede neural convolucional (CNN)** para
classificar imagens de **maçãs** e **tomates**.\
A ideia é carregar o dataset, preparar as imagens e treinar o modelo
para distinguir entre as duas classes.

------------------------------------------------------------------------


## ⚙️ Tecnologias utilizadas

-   Python\
-   TensorFlow / Keras\
-   NumPy\
-   Pandas\
-   Matplotlib\
-   Seaborn\
-   Scikit-learn
-   [apples_or_tomatoes.zip](https://github.com/user-attachments/files/22407491/apples_or_tomatoes.zip.zip)
------------------------------------------------------------------------

## 📂 Estrutura do dataset

O dataset precisa estar em formato `.zip` com a seguinte estrutura:

    dataset/
    │── train/
    │   ├── apples/
    │   ├── tomatoes/
    │
    └── test/
        ├── apples/
        ├── tomatoes/

No Google Colab, o arquivo `.zip` é carregado manualmente e extraído
dentro de `/content/dataset`.

------------------------------------------------------------------------

## 🚀 Como executar

1.  Abrir o projeto no **Google Colab**.\
2.  Rodar a primeira célula para fazer o upload do dataset `.zip`.\
3.  O código vai extrair o dataset e criar os geradores de treino e
    teste.\
4.  A CNN será treinada por **20 épocas**.\
5.  Ao final, o modelo mostra:
    -   Acurácia\
    -   AUC\
    -   Classification report\
    -   Gráficos de **Accuracy**, **Loss** e **AUC** por época

------------------------------------------------------------------------

## 🧠 Estrutura do modelo

A CNN foi construída com as seguintes camadas:\
- Conv2D (32 filtros) + MaxPooling2D\
- Conv2D (64 filtros) + MaxPooling2D\
- Conv2D (128 filtros) + MaxPooling2D\
- Conv2D (256 filtros) + MaxPooling2D\
- Flatten\
- Dropout (50%)\
- Dense (512 neurônios, ReLU)\
- Dense (1 neurônio, Sigmoid)

O otimizador utilizado foi **Adam** com `learning_rate=0.0001`.

------------------------------------------------------------------------

## 📊 Resultados esperados

-   Métricas de treino e validação a cada época\
-   Classification report (Precision, Recall, F1)\
-   Confusion matrix\
-   Gráficos de aprendizado

------------------------------------------------------------------------

## 🔮 Possíveis melhorias

-   Usar **data augmentation** para aumentar a diversidade do treino\
-   Testar **transfer learning** (ex.: VGG16, ResNet50)\
-   Implementar **early stopping** para evitar overfitting\
-   Salvar e carregar o modelo treinado (`.h5`)

------------------------------------------------------------------------

⚡ Projeto ideal para praticar **redes neurais convolucionais** e
aprender sobre **classificação de imagens**.
