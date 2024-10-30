# n2_martim_ciencia_de_dados

Em resolução do problema, foi feito em linguagem Python no Google Colab (Notebooks) o código necessário para rodar a aplicação.  
No link (público): [Pasta do Projeto no Google Drive](https://drive.google.com/drive/folders/1-JMit_RuiWThvjjQS3-QgdHMy62sKIpa?usp=sharing),  
podemos observar a pasta principal: `N2_MARTIM_ELEIÇÕES`, o arquivo `N2_MARTIM.ipynb`, o `mapa_prefeitos_2024` (gerado pelo Colab),  
o arquivo `consulta_cand_colunas` (para entendimento do projeto) e o exercício passado pelo professor.  

Além do mais, temos a pasta `datasheet`, onde estão todos os dados utilizados para a aplicação.

Dentro do datasheet, temos as pastas com os CSVs de:
- `propostas_governo_sc`
- `bem_candidato_2024`
- `consulta_cand_2024`
- `consulta_coligacao_2024`
- `rede_social_candidato_2024`

Além dessas pastas com os arquivos CSV, também temos o arquivo `Latitude_Longitude` dos municípios do Brasil e o `resultado_rede_social`.

Todos esses arquivos são essenciais para o entendimento, a qualidade e a funcionalidade do arquivo Python.

## Como funciona o aplicativo?

### 1. Bibliotecas necessárias

Para rodar este projeto, instale as seguintes bibliotecas:
```python
import os
import pandas as pd
from google.colab import drive
