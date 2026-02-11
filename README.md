# Modelo de classificação de imagens usando transfer-Learning
Modelo de classificação de imagens capaz de diferenciar entre gatos e cães, utilizando técnicas de Deep Learning e Transfer Learning

# Classificação de Imagens de Gatos e Cães usando Transfer Learning com VGG16

### Introdução:

O presente projeto tem como objetivo construir um modelo de classificação de imagens capaz de diferenciar entre gatos e cães, utilizando técnicas de Deep Learning e Transfer Learning.

O objetivo final é demonstrar como Transfer Learning pode ser aplicado em problemas reais de classificação de imagens, aproveitando redes profundas pré-treinadas para reduzir tempo de treinamento e melhorar a acurácia mesmo com datasets limitados.


### Dataset utilizado
Foi empregado o conjunto de dados Cats vs Dogs, [disponibilizado pela Microsoft](https://www.microsoft.com/en-us/download/details.aspx?id=54765) e amplamente utilizado em competições de aprendizado de máquina.

O dataset contém aproximadamente 25 mil imagens divididas em duas classes: “Cat” e “Dog”. Como algumas imagens apresentavam problemas de integridade ou canais não compatíveis, foi realizado um pré-processamento cuidadoso para remover imagens corrompidas e padronizar o formato das imagens para 3 canais RGB e tamanho fixo de 224x224 pixels.

### Redes Neurais Utilizadas

Foi utilizada a rede pré-treinada VGG16, conhecida por sua robustez em tarefas de classificação, principalmente em visão computacional. Apenas a camada de classificação final foi ajustada para o problema binário específico, enquanto as demais camadas permaneceram congeladas, aproveitando os pesos pré-treinados na ImageNet.


### Particionamento e Pré-processamento
O projeto utilizou:

- Tamanho do dataset usado para treino/val/test (10% cada).

- Normalização de imagens e preprocessamento compatível com VGG16.

- Avaliação de acurácia, perda, matriz de confusão e outras métricas, além de visualização de predições com probabilidades por classe.

### Tecnologias utilizadas
O projeto foi desenvolvido em Python utilizando o framework TensorFlow/Keras para construção e treinamento de redes neurais. Para pré-processamento e manipulação de imagens foram empregadas bibliotecas como PIL e NumPy, enquanto Matplotlib foi utilizada para visualização de imagens e métricas de desempenho. Para avaliação de resultados, foram usadas métricas do Scikit-learn (matriz de confusão, recall, F1-score) e JSON para armazenamento dos históricos de treino. Funções padrão de OS e Random foram utilizadas para navegação em diretórios e seleção aleatória de imagens.

<img src="https://github.com/monicaneli/Transfer-Learning/blob/3afa246b70e4ce098476bb5965cd5446356a0021/resultado_classifica%C3%A7%C3%A3o_gatos_e_cachorros.png" />

