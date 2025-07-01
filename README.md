# Poder de Compra do Salário-Mínimo: Uma Análise Comparativa Internacional

Este projeto apresenta uma análise comparativa do poder de compra do salário-mínimo em diversos países, com foco na quantidade de alimentos básicos que podem ser adquiridos. A aplicação interativa, desenvolvida em Streamlit, permite explorar visualizações de dados que revelam disparidades econômicas, a relação entre PIB per capita e poder de compra, e a posição do Brasil no cenário global.

## 📊 Visualizações Chave

O aplicativo oferece as seguintes visualizações interativas:

1.  **Salário Mínimo Mensal por País (em USD$)**: Uma comparação direta dos salários mínimos entre os países selecionados.
2.  **Poder de Compra Médio por País (Ranking Geral)**: Classificação dos países com base na quantidade média de produtos básicos que o salário mínimo pode adquirir.
3.  **Poder de Compra Detalhado por Produto e País**: Detalha quantas unidades de cada produto selecionado o salário mínimo de cada país consegue comprar.
4.  **Poder de Compra Médio de Alimentos vs. PIB Per Capita**: Um gráfico de dispersão que investiga a correlação entre a riqueza do país (PIB per capita) e a capacidade de compra do salário mínimo.
5.  **Grouping: Poder de Compra Médio por Categoria de País**: Análise comparativa do poder de compra médio entre categorias de países (Economias Desenvolvidas, Grandes Economias em Ascensão e Economias de Mercado Emergentes).
6.  **Brasil no Cenário Global: Poder de Compra por Categoria de País**: Destaca a posição do Brasil em relação aos diferentes grupos econômicos.
7.  **Mapa Mundial do Poder de Compra Médio**: Uma representação geográfica da distribuição do poder de compra do salário mínimo globalmente.

## 🎯 Perguntas de Pesquisa e Análise

O projeto busca responder às seguintes perguntas:

* Qual a quantidade de alimentos básicos que o salário-mínimo compra em diferentes países?
* Existe uma correlação clara entre o PIB per capita de um país e o poder de compra de alimentos do salário-mínimo?
* Como o Brasil se compara a economias desenvolvidas e a outras economias emergentes?
* Qual a diferença no poder de compra médio de alimentos entre as categorias de países ('Desenvolvidos', 'Em Ascensão' e 'Emergentes')?

## 🚀 Como Rodar o Projeto Localmente

O projeto foi configurado para ser executado no Google Colab, utilizando pyngrok para expor o aplicativo Streamlit publicamente.

### 1. Abrir o notebook

Faça o upload do arquivo app_economia.ipynb para o seu Google Drive e abra-o no Google Colab.

### 2. Configurar o Ngrok Auth Token

Você precisará de um Auth Token do Ngrok. Cadastre-se em ngrok.com e copie seu token na seção "Your Authtoken".
NGROK_AUTH_TOKEN = "SEU_AUTHTOKEN_REAL_AQUI" # <<<<<< AQUI É ONDE VOCÊ COLA O TOKEN

### 3. Estrutura de Pastas dos Dados

Certifique-se de que seus arquivos de dados e mapa estejam nas seguintes pastas dentro do seu Google Drive, acessíveis pelo Colab:

Meu Drive/
└── Economia/
    ├── app_economia.py
    ├── dados/
    │   ├── dados_economia(Alimentos).csv
    │   ├── dados_economia(salário-mínimo).csv
    │   └── dados_economia(PIB).csv
    └── mapa/
        ├── ne_110m_admin_0_countries.shp
        ├── ne_110m_admin_0_countries.shx
        ├── ne_110m_admin_0_countries.dbf
        ├── ne_110m_admin_0_countries.prj
        └── ne_110m_admin_0_countries.cpg

O notebook já configura o app.py para ser salvo em /content/drive/MyDrive/Economia/app.py, e os diretórios DADOS_DIR e MAPA_DIR são definidos para /content/drive/MyDrive/Economia/dados e /content/drive/MyDrive/Economia/mapa respectivamente.

### 4. Rodar o aplicativo 

Execute todas as células do notebook sequencialmente. A última célula irá iniciar o servidor Streamlit e fornecer um URL público do Ngrok para acessar o aplicativo.

### 📚 Fontes dos Dados:

* Numbeo (preços de alimentos por país): https://www.numbeo.com/cost-of-living/. 
* ILO (salário-mínimo por país): https://ilostat.ilo.org/topics/wages/ 
* Banco Mundial – Indicadores econômicos: https://data.worldbank.org 

