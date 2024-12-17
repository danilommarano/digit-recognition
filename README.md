---
title: Digit Recognition
emoji: 🔢
colorFrom: blue
colorTo: green
sdk: gradio
sdk_version: 3.50.2
app_file: app.py
pinned: false
license: cc
---

# Modelo de Classificação de Dígitos MNIST usando TensorFlow

Este repositório contém os arquivos necessários para o desenvolvimento, treinamento e aplicação de um modelo de **Rede Neural Convolucional (CNN)** para classificar imagens do dataset **MNIST**, utilizando **TensorFlow/Keras**.

### **Arquivos do Repositório**

1. **mnist_model_process.ipynb**

   - Notebook que descreve passo a passo a criação, o treinamento e o salvamento do modelo CNN.
   - Inclui todas as etapas, desde o pré-processamento dos dados até a construção da rede e avaliação do modelo.

2. **model.py**

   - Contém o código Python responsável pela construção, treinamento e salvamento do modelo CNN.
   - É uma versão simplificada do notebook, ideal para execução em scripts automatizados.

3. **app.py**
   - Implementa um **dashboard interativo** no qual o usuário pode desenhar dígitos à mão usando o mouse.
   - O modelo treinado é carregado para testar os dígitos desenhados em tempo real, exibindo a previsão diretamente na interface.

### Como usar?

Para usar o modelo de forma local basta baixar as dependências e rodar o arquivo model.py. Assim um novo modelo será treinado e salvo como model.h5.

```python
pip install -r requirements.txt
python model.py
```

Agora para usar o dashboard que testa o modelo de forma interativa, basta executar o arquivo app:

```python
python app.py
```

E assim você terá um dashboard que é capaz de descobrir qual digito você escreveu.
