# Percentual de Gordura em Cortes de Carne

Projeto desenvolvido para a disciplina **Clube de Programação** com o objetivo de estimar o percentual de gordura presente em cortes de carne utilizando técnicas de Processamento Digital de Imagens e Machine Learning.

## Autores

- Samuel Hermnay - samuelhermny1012@gmail.com
- Johanna Liza Herrera - johannaliza8@gmail.com

## Objetivo

O projeto realiza a análise de imagens de cortes de carne para identificar regiões de gordura e calcular sua porcentagem em relação à área total da peça.

Foram implementadas duas abordagens:

- Processamento Digital de Imagens utilizando OpenCV.
- Machine Learning utilizando MLPClassifier (Scikit-Learn).

---

## Estrutura do Projeto

```text
PERCENTUAL-GORDURA-CARNE
│
├── codigos
│   ├── opencv_apresentacao.ipynb
│   └── machine_learning_apresentacao.ipynb
│
├── imagens
│   ├── 01.png
│   ├── 02.png
│   ├── ...
│
├── open_cv
│   ├── imagens de saída geradas pelo OpenCV
│
├── machine_learning
│   ├── modelo
│   │   └── modelo_gordura.pkl
│   ├── imagens de saída geradas pelo Machine Learning
│
├── Clube de programação.pdf
├── Clube de programação.pptx
└── README.md
```

---

## Desenvolvimento

Todo o projeto foi desenvolvido e executado utilizando o **Google Colab**.

Os notebooks contendo os códigos-fonte são:

### 1. OpenCV

Arquivo:

```text
codigos/opencv_apresentacao.ipynb
```

Nesta abordagem foram utilizadas técnicas de processamento digital de imagens para:

- Carregar a imagem.
- Converter para o espaço de cores HSV.
- Remover o fundo branco.
- Identificar regiões de gordura através de faixas de cores.
- Aplicar filtros para redução de ruídos.
- Calcular o percentual de gordura.
- Gerar imagens com as regiões detectadas.

---

### 2. Machine Learning

Arquivo:

```text
codigos/machine_learning_apresentacao.ipynb
```

Nesta abordagem foi utilizada uma Rede Neural do tipo MLP (Multi-Layer Perceptron) através da biblioteca Scikit-Learn.

O processo consiste em:

- Treinar um modelo utilizando exemplos de carne e gordura.
- Salvar o modelo treinado em arquivo `.pkl`.
- Carregar o modelo treinado.
- Classificar os pixels da imagem.
- Identificar as regiões de gordura.
- Calcular o percentual de gordura.
- Gerar imagens com o resultado da classificação.

---

## Tecnologias Utilizadas

- Python
- OpenCV
- NumPy
- Scikit-Learn
- Google Colab

---

## Resultados

Para cada imagem analisada são gerados:

- Imagem original.
- Máscara de gordura identificada.
- Imagem final com as regiões de gordura destacadas em vermelho.

Os resultados produzidos por cada abordagem podem ser encontrados nas pastas:

```text
open_cv/
machine_learning/
```

---

## Como Executar

- O projeto foi desenvolvido no Google Colab com as imagens no googgle drive.
- Para executar no seu pc local, altere nas **Configurações Iniciais** de cada projeto o endereço **path** abaixo:<br>
  ```bash
  path = "/content/drive/MyDrive/Clube de Programacao-2026/Apresentacao/"
  ```

## 1. Criar a seguinte esturura de pastas

```text
SUA_PASTA_PRINCIPAL
│
├── imagens
│
├── open_cv
│
├── machine_learning
│   ├── modelo
│
```

### 2. Abrir um dos notebooks

- `codigos/opencv_apresentacao.ipynb`
- `codigos/machine_learning_apresentacao.ipynb`

### 3.A Para OpenCV, clicar em Run All

### 3.B Para Machine Lerning, primeira vez clicar em Run All

- As demais vezes só execute o último bloco de (2.4) Testes
