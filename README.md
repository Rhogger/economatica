# 📊 Análise de Dados Economatica

Projeto de análise de dados financeiros da Economatica para pós-graduação em Data Science da UniRV.

## 👥 Equipe

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat&logoSize=15)](https://www.linkedin.com/in/rhogger-fs/) - **Rhogger Freitas Silva**
<br>
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat&logoSize=15)](https://www.linkedin.com/in/josehenriqve/) - **José Henrique Queiroz de Souza**
<br>
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat&logoSize=15)](https://www.linkedin.com/in/mateusabreucn/) - **Mateus Abreu da Cunha Nascimento**
<br>
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat&logoSize=15)](https://www.linkedin.com/in/felipeperetti/) - **Felipe Peretti**

## 📋 Descrição do Projeto

Este projeto realiza análise de dados financeiros provenientes da base Economatica, seguindo as seguintes etapas:

- 🧹 Limpeza de dados
- 🔍 Análise exploratória de dados financeiros  
- 📊 Visualização de insights financeiros
- 📈 Pré-processamento dos dados para modelagem
- 🤖 Modelagem preditiva para **classificação de variação do valor de mercado** (positiva e negativa) de ações

## 🛠️ Tecnologias Utilizadas

- **Python 3.11.13**
- **Pandas** - Manipulação de dados
- **NumPy** - Operações numéricas
- **Scikit-learn** - Machine Learning e normalização
- **PyCaret** - AutoML para comparação de modelos
- **Matplotlib/Seaborn** - Visualização de dados
- **Jupyter Notebook** - Ambiente de desenvolvimento

## ⚙️ Configuração do Ambiente

### 📱 Google Colab (Recomendado para Iniciantes)

1. **Altere o Runtime**: para Python 3.11 (versão 2025.07)
   - Menu: `Runtime` → `Change runtime type` → Selecione a versão "2025.07"
   - [Documentação oficial](https://research.google.com/colaboratory/runtime-version-faq.html#2025.07)

2. **Faça o download do notebook e o upload manualmente**:
   - Acesse `src/notebooks/analise_dados_economatica.ipynb` e baixe o arquivo.
   - Faça o upload do notebook no colab.
   - Execute as células sequencialmente até a instação de dependências.

3. **Após a instalação das dependências**: Reinicie a sessão do runtime.

### 💻 Ambiente Local

**⚠️ Importante**:

- Em todas as alternativas, é necessário o Python na versão **3.11.13**, considere utilizar o [**asdf**](https://asdf-vm.com/) para gerenciamento de versão de linguagens/frameworks.

- Abra a workspace no VS Code:

```bash
code economatica.code-workspace
```

- Crie um arquivo `.env` na raiz do projeto com o conteúdo:

```bash
GOOGLE_COLAB_RUNTIME=false
```

**Obs:** Caso não queira utilizar o Jupyter Notebook, não precisa executar o comando `jupyter notebook`

#### Opção 1: Pipenv (Recomendado)

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/economatica.git
cd economatica

# Instale o pipenv se não tiver
pip install pipenv

# Instale as dependências
pipenv install

# Ative o ambiente virtual
pipenv shell

# Inicie o Jupyter
jupyter notebook
```

#### Opção 2: pip + venv

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/economatica.git
cd economatica

# Crie ambiente virtual
python -m venv venv

# Ative o ambiente virtual
# Linux/Mac:
source venv/bin/activate
# Windows:
# venv\Scripts\activate

# Instale as dependências
pip install -r requirements.txt

# Inicie o Jupyter
jupyter notebook
```

#### Opção 3: pip direto

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/economatica.git
cd economatica

# Instale as dependências
pip install -r requirements.txt

# Inicie o Jupyter
jupyter notebook
```

## 🚀 Como Executar

1. **Configure o ambiente** seguindo uma das opções acima
2. **Abra o Jupyter Notebook** (ou use Google Colab ou VS Code)
3. **Navegue até** `src/notebooks/analise_dados_economatica.ipynb`
4. **Execute as células** sequencialmente

## 📊 Datasets

### Dados de Entrada

- `df_economatica.csv` - Dataset original da Economatica

### Dados Processados

- `df_economatica_limpo.csv` - Dados após limpeza inicial
- `df_economatica_pre_processado_normalizado.csv` - Dados normalizados
