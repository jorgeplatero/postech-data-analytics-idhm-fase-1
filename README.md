# Aplicativo Web com Indicadores do IDHM de São Paulo de 2010

O Índice de Desenvolvimento Humano Municipal (IDHM) é uma medida composta que avalia o desenvolvimento humano em três dimensões: **longevidade, educação e renda**. Este projeto é um dashboard interativo construído com **Streamlit** para visualizar e analisar esses indicadores nos municípios do Estado de São Paulo com base nos dados do censo de 2010.

### Pré-requisitos

Certifique-se de ter o Python 3.11 instalado em seu sistema.

Instale o suporte ao ambiente virtual:

```bash
sudo apt update && sudo apt install python3.11-venv
```

### Instalação

Clone o repositório e instale as dependências:

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
| **Frontend/App** | **Streamlit** | `1.23.1` | Framework para desenvolvimento de aplicativo web |
| **Análise de Dados** | **Pandas** | `2.0.2` | Biblioteca para manipulação de dados |
| **Visualização** | **Plotly** | `5.15.0` | Biblioteca para criação de gráficos dinâmicos e interativos |
| **Comunicação** | **Requests** | `2.31.0` | Biblioteca para requisições HTTP e consumo de API ||
| **Linguagem** | **Python** | `>=3.11` | Linguagem para desenvolvimento de scripts |
| **Gerenciamento** | **Venv** | `-` | Gerenciador de ambientes virtuais para isolamento de dependências |

### Fontes de Dados

O fluxo de dados utiliza a base estatística oficial do IPEA (Ipeadata) referente ao IDH 2010.

Link para a base de dados: https://www.ipea.gov.br/ipeageo/arquivos/bases/IDH_2010.xls

### Deploy

O aplicativo web está disponível via Streamlit Cloud.

Link para o aplicativo web: https://postechidhmfase1-gefaxadhrrgxvcmpaglmse.streamlit.app/
