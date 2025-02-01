# Análise de Dados e Modelagem Preditiva para Preço de Apartamentos no Airbnb

## Visão Geral
Este projeto realiza uma análise exploratória dos dados (EDA) e desenvolve um modelo de previsão de preços de apartamentos listados no Airbnb. O objetivo é identificar padrões e fatores que influenciam no preço dos imóveis e fornecer recomendações para investidores.

## Estrutura do Repositório
```
/
├── data/  # Contém os datasets utilizados
├── notebooks/  # Jupyter Notebooks com as análises exploratórias e modelagem
├── models/  # Contém o modelo salvo (.pkl)
├── reports/  # Relatórios de análise estatística e EDA
├── requirements.txt  # Lista de dependências do projeto
├── README.md  # Este arquivo explicativo
└── video/  # Link para o vídeo explicativo
```

## Instalação e Execução
1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd nome-do-repositorio
   ```
3. Crie um ambiente virtual e instale as dependências:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate  # Windows
   pip install -r requirements.txt
   ```
4. Execute a análise exploratória e a modelagem (Jupyter Notebook):
   ```bash
   jupyter notebook
   ```

## Análise Exploratória (EDA)
A análise exploratória demonstrou:
- Correlações entre variáveis como bairro, tipo de acomodação e preço.
- Impacto do número mínimo de noites e disponibilidade no preço.
- Padrões em nomes de acomodações para locais mais caros.
- Hipóteses de negócio sobre investimento ideal em propriedades para aluguel.

Os insights detalhados estão documentados no relatório de EDA (disponível na pasta `reports/`).

## Modelagem Preditiva
- Tipo de problema: **Regressão**.
- Modelo selecionado: [Melhor modelo escolhido]
- Métrica de avaliação: [Métrica utilizada, ex.: RMSE]
- Explicação das variáveis utilizadas e transformações aplicadas.

## Previsão de Preço
Para um apartamento com as seguintes características:
```
{'id': 2595,
 'nome': 'Skylit Midtown Castle',
 'host_id': 2845,
 'host_name': 'Jennifer',
 'bairro_group': 'Manhattan',
 'bairro': 'Midtown',
 'latitude': 40.75362,
 'longitude': -73.98377,
 'room_type': 'Entire home/apt',
 'minimo_noites': 1,
 'numero_de_reviews': 45,
 'ultima_review': '2019-05-21',
 'reviews_por_mes': 0.38,
 'calculado_host_listings_count': 2,
 'disponibilidade_365': 355}
```
O modelo estima um preço de **[valor previsto]**.

## Modelo Treinado
O modelo treinado foi salvo no formato `.pkl` e pode ser carregado da seguinte forma:
```python
import pickle
with open('models/modelo.pkl', 'rb') as file:
    modelo = pickle.load(file)
```

## Relatórios
Os relatórios das análises estatísticas e do EDA estão disponíveis em PDF e Jupyter Notebook na pasta `reports/`.

## Vídeo Explicativo
O vídeo explicando o desenvolvimento do projeto pode ser acessado [aqui](link-do-video).

## Contato
Caso tenha dúvidas ou sugestões, entre em contato via [seu e-mail ou LinkedIn].

