# Projeto de Modelagem Estatística: Análise de Sono em Mamíferos 💤

Este repositório contém o projeto prático do 2º Bimestre da disciplina de **Modelagem Estatística** do curso de Ciência da Computação. O objetivo é aplicar técnicas de Regressão e Classificação para analisar padrões de sono em diferentes espécies de mamíferos.

## 🎯 Objetivos do Projeto
O projeto utiliza o dataset **Sleep in Mammals** para resolver dois problemas de negócio:
1.  **Regressão:** Prever a duração total do sono (`total_sleep`) com base em características biológicas e ecológicas (peso, perigo, etc.).
2.  **Classificação:** Categorizar os animais em "Short Sleepers" ou "Long Sleepers" (variável `sleep_class`), identificando padrões de comportamento.

## 🛠️ Ferramentas Utilizadas
O projeto foi desenvolvido em **Python 3.11.9** utilizando as seguintes bibliotecas:
* **Manipulação de Dados:** Pandas, Numpy.
* **Visualização:** Seaborn, Matplotlib.
* **Estatística e Modelagem:** Statsmodels, Scikit-learn.
* **AutoML e Otimização:** PyCaret (O PyCaret não funciona em python 3.12+).

## 📂 Estrutura do Repositório
* `Projeto_Modelagem.ipynb`: Jupyter Notebook contendo todo o código (EDA, Limpeza, Modelagem e Relatório).
* `dataset_2191_sleep.csv`: Arquivo de dados bruto (Fonte: OpenML/Kaggle).
* `requirements.txt`: Lista de dependências para reprodução do ambiente.
* `README.md`: Documentação do projeto.

## 🚀 Como Executar
Para rodar este projeto localmente, siga os passos abaixo:

1.  **Clone o repositório:**
```bash
    git clone https://github.com/ffelipef/projetoModelagem.git
    cd NOME_DO_REPO
```

2.  **Instale as dependências:**
    Recomenda-se o uso de um ambiente virtual (venv ou conda).
```bash
    pip install -r requirements.txt
```

3.  **Execute o Notebook:**
```bash
    jupyter notebook Projeto_Modelagem.ipynb
```
    *Nota: Se estiver usando o Google Colab, basta fazer o upload do notebook e do arquivo csv para o ambiente.*

## 📊 Resultados Principais
* A **Análise Exploratória** revelou que o **Índice de Perigo** (`danger_index`) possui forte correlação negativa com o tempo de sono.
* Na etapa de **Regressão**, modelos não-lineares (Polinomiais e Random Forest via PyCaret) superaram a Regressão Linear simples.
* Na **Classificação**, foi possível prever com alta acurácia se um animal dorme muito ou pouco baseado apenas em seu peso e risco de predação.

## 📝 Autores
**Felipe de Freitas da Silva**
**Benjamin Yuji Suzuki**
