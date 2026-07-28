## 📌 Descrição

A seguinte atividade teve como objetivo elaborar um **Data Lake local** sobre os dados de Jogos Olímpicos de Verão e Inverno (medalhas, atletas e modalidades), organizando em três camadas:

* **raw** → dados brutos
* **bronze** → dados tratados
* **gold** → visualizações

Em cada camada foram definidos metadados para visualizar a estrutura geral da base de dados nas etapas de carregamento, pré-processamento e análise 


Os dados foram obtidos de dois datasets: _Historical Data from the Olympics_ e _Paris 2024 Olympic Summer Games_. Disponíveis em:
  - https://basedosdados.org/dataset/62f8cb83-ac37-48be-874b-b94dd92d3e2b?table=567b1ccd-d8c2-4616-bacb-cf5c0e7b8d89
  - https://www.kaggle.com/datasets/piterfm/paris-2024-olympic-summer-games/data

## 🗂️ Sobre as pastas

### RAW
Contêm os dados que foram carregados (sem processamento) e seus metadados

### BRONZE
Contêm os dados processados em etapas como:
* Conversão CSV → Parquet
* Padronização de colunas
* Separação de `edition` em `Summer Olympics` e `Winter Olympics`
* Integração dos datasets

### GOLD
Contêm os dados após análise e gráficos gerados para:

**Medalhas**
* Ranking de países (Top 50)

**Modalidades**
* Quantidade de eventos únicos por esporte

**Atletas**
* Distribuição por sexo

