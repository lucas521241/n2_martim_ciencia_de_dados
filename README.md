# AVALIAÇÃO N2 - CIÊNCIA DE DADOS

## Equipe
- Lucas Josué Schneider
- João Pedro Papp
- Antonio Marcos Siqueira

## Faculdade
Católica SC - Jaraguá do Sul

## Curso
Engenharia de Software, 8ª fase

## Matéria
Ciência de Dados

## Professor
Martim Dietterle

---

Em resolução do problema, foi feito em linguagem Python no Google Colab (Notebooks) o código necessário para rodar a aplicação.  
No link (público): Pasta do Projeto no Google Drive,  
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
!pip install pandas
!pip install numpy
!pip install matplotlib
!pip install seaborn
!pip install google.colab
!pip install PyPDF2
!pip install scikit-learn
!pip install folium
```

### 2. Leitura dos Datasheets

O código inicial foi desenvolvido para montar o Google Drive, definir o caminho da pasta raiz onde os CSVs estão localizados e carregar todos os arquivos CSV de forma correta. Funções específicas foram criadas para lidar com diferentes tipos de arquivos e possíveis erros de leitura.

### Questões Respondidas

#### Questão 1
- **Objetivo**: Verificar se o prefeito eleito é o que declarou mais bens em cada município.
- **Passos**:
  1. Carregar dados de candidatos e bens.
  2. Fazer merge dos dados.
  3. Filtrar candidatos eleitos para prefeito.
  4. Calcular a soma dos bens declarados por candidato.
  5. Verificar se o prefeito eleito é o que declarou mais bens.

#### Questão 2
- **Objetivo**: Analisar coligações e partidos.
- **Passos**:
  1. Carregar dados de candidatos.
  2. Filtrar candidatos eleitos.
  3. Contar o número de partidos em cada coligação.
  4. Agrupar e ordenar coligações por número de candidatos eleitos e número de partidos.

#### Questão 3
- **Objetivo**: Identificar o partido com mais candidatos em cada UF.
- **Passos**:
  1. Agrupar dados por estado (UF) e partido.
  2. Contar o número de candidatos por partido em cada UF.
  3. Identificar o partido com mais candidatos em cada UF.

#### Questão 4
- **Objetivo**: Verificar a tendência de partidos em cada estado.
- **Passos**:
  1. Contar o número de candidatos por partido e UF.
  2. Verificar a tendência de partidos em cada estado com base em um limite de candidatos.

#### Questão 5
- **Objetivo**: Encontrar o maior partido por UF.
- **Passos**:
  1. Contar o número de candidatos distintos por partido e UF.
  2. Identificar o maior partido por UF.

#### Questão 6
- **Objetivo**: Analisar candidatos indígenas e quilombolas.
- **Passos**:
  1. Filtrar candidatos indígenas e quilombolas.
  2. Contar o número de candidatos por região.
  3. Identificar a região com mais candidatos indígenas e quilombolas.

#### Questão 7
- **Objetivo**: Analisar redes sociais dos candidatos.
- **Passos**:
  1. Carregar dados de redes sociais e candidatos.
  2. Extrair a rede social do URL.
  3. Juntar dados de redes sociais com dados de candidatos.
  4. Exportar resultados para um arquivo CSV.

#### Questão 8
- **Objetivo**: Identificar termos mais frequentes em propostas de governo.
- **Passos**:
  1. Extrair e limpar texto de arquivos PDF.
  2. Usar um vetor de contagem para identificar termos mais frequentes nos textos.

#### Questão 9
- **Objetivo**: Criar um mapa interativo com prefeitos eleitos.
- **Passos**:
  1. Carregar dados de candidatos e coordenadas geográficas.
  2. Filtrar prefeitos eleitos.
  3. Mesclar dados de candidatos com coordenadas.
  4. Criar um mapa interativo com marcadores para os prefeitos eleitos.

---

Este projeto foi desenvolvido para analisar dados eleitorais e responder a diversas questões relacionadas às eleições de 2024. Cada questão foi abordada com um conjunto específico de passos e técnicas de análise de dados.



