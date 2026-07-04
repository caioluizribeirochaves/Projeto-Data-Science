# 🏖️ Projeto Data Science: Previsão de Preços de Estadia no Airbnb - Rio de Janeiro

Este é um projeto de Ciência de Dados de ponta a ponta que visa prever o preço de diárias de imóveis do Airbnb na cidade do Rio de Janeiro. O projeto engloba desde o tratamento massivo dos dados brutos, análise exploratória, treinamento de modelo preditivo até a criação de um aplicativo web interativo para o usuário final.

---

## 📊 Origem dos Dados

Os dados utilizados neste projeto foram obtidos no Kaggle, através do dataset público disponibilizado por Allan Bruno:
🔗 [Airbnb Rio de Janeiro Dataset - Kaggle](https://www.kaggle.com/datasets/allanbruno/airbnb-rio-de-janeiro)

---

## 🛠️ Etapas do Projeto

O pipeline do projeto foi estruturado em três grandes fases:

### 1. Limpeza e Tratamento de Dados (Data Cleaning)
* **Filtragem de Outliers:** Remoção de valores discrepantes de preços e quantidades para evitar distorções no modelo.
* **Tratamento de Variáveis Booleanas:** Conversão de colunas de texto estrito (`'t'` e `'f'`) para formato numérico binário (`1` e `0`) em colunas como `host_is_superhost` e `instant_bookable`.
* **Codificação de Variáveis Categóricas:** Aplicação de *One-Hot Encoding* (`pd.get_dummies`) para transformar categorias textuais (tipos de imóvel, quartos, políticas de cancelamento) em dados inteligíveis para o algoritmo.

### 2. Modelagem Preditiva (Machine Learning)
* Treinamento de um três modelos para avaliar o que se sairia melhor nessa situação, modelos utilizados **LinearRegression/RandomForest/ExtraTrees** (Scikit-Learn).
* Alinhamento rigoroso das colunas de entrada para garantir previsões consistentes com os dados de treino.
* Exportação do modelo treinado (`modelo.joblib`).

### 3. Deploy da Aplicação (Web App)
* Construção de uma interface de usuário interativa e limpa utilizando o **Streamlit**.
* Inputs customizados para o usuário preencher dados geográficos (latitude/longitude), características do imóvel (banheiros, quartos, camas, amenidades) e regras contratuais.

---

## ⚙️ Tecnologias e Bibliotecas Utilizadas

| Tecnologia/Biblioteca | Função no Projeto |
| :--- | :--- |
| **Python** | Linguagem principal do projeto |
| **Pandas** | Manipulação, limpeza e tratamento dos dados |
| **NumPy** | Operações matemáticas e suporte matricial |
| **Scikit-Learn** | Criação, validação e treinamento do modelo de Machine Learning |
| **Joblib** | Serialização e salvamento do modelo treinado em disco |
| **Streamlit** | Desenvolvimento do aplicativo web de Deploy |

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
Certifique-se de ter o Python instalado. É recomendado o uso de um ambiente virtual (`venv`).

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/caioluizribeirochaves/Projeto-Data-Science.git](https://github.com/caioluizribeirochaves/Projeto-Data-Science.git)
   cd Projeto-Data-Science

## 💡 Preview do Projeto

```markdown
![Preview do App](GIF-FUNCIONAMENTO.GIF)

