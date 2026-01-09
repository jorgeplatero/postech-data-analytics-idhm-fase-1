# Aplicativo Web com Indicadores do IDHM de São Paulo em 2010

O Índice de Desenvolvimento Humano Municipal (IDHM) é uma medida composta que avalia o desenvolvimento humano em três dimensões: **longevidade, educação e renda**. Este projeto é um dashboard interativo construído com **Streamlit** para visualizar e analisar esses indicadores nos municípios do Estado de São Paulo com base nos dados do censo de 2010.

### Pré-requisitos

Certifique-se de ter o Python 3.11 instalado em seu sistema.

Instale o suporte ao ambiente virtual:

```bash
sudo apt update && sudo apt install python3.11-venv
```

### Instalação

Clone o repositório, crie o ambiente virtual e instale as dependências:

```bash
#clonar o repositório
git clone https://github.com/jorgeplatero/postech-idhm-fase-1.git
cd postech-data-analytics-fase-1-idhm-web-app

#criar o ambiente virtual
python -m venv venv

#ativar o ambiente virtual
source venv/bin/activate

#instalar as dependências
pip install -r requirements.txt
```

### Como Rodar a Aplicação

Com o ambiente virtual ativado, execute o comando abaixo para iniciar o Streamlit:

```bash
streamlit run app.py
```

### Tecnologias

| Componente | Tecnologia | Versão | Descrição |
| :--- | :--- | :--- | :--- |
| **Frontend/App** | **Streamlit** | `1.23.1` | Framework utilizado para a construção da interface interativa e dashboard |
| **Análise de Dados** | **Pandas** | `2.0.2` | Biblioteca utilizada para manipulação de dataframes e estruturação de tabelas |
| **Visualização** | **Plotly** | `5.15.0` | Biblioteca para criação de gráficos dinâmicos e interativos |
| **Comunicação** | **Requests** | `2.31.0` | Biblioteca para requisições HTTP e integração de dados |
| **Linguagem** | **Python** | `>=3.11` | Linguagem de programação base para o desenvolvimento dos scripts |
| **Gerenciamento** | **Venv** | `-` | Gerenciador de pacotes e ambientes virtuais utilizado para garantir a reprodutibilidade das dependências do projeto |

### Integrações

O fluxo de dados utiliza a base estatística oficial do IPEA (Ipeadata) referente ao IDH 2010.
Os dados brutos podem ser consultados aqui: [IDH_2010.xls](https://www.ipea.gov.br/ipeageo/arquivos/bases/IDH_2010.xls)

### Deploy

O dashboard está disponível via Streamlit Cloud.

Link para o aplicativo: [https://postechidhmfase1.streamlit.app/](https://postechidhmfase1-gefaxadhrrgxvcmpaglmse.streamlit.app/)
