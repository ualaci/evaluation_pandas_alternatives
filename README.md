# Comparação de Desempenho entre Bibliotecas de DataFrames

Este projeto compara o desempenho de diferentes bibliotecas de processamento de dados em Python, como Pandas, Polars, Vaex e Datatable. Ele mede o tempo de execução e uso de memória para operações comuns como leitura de arquivos CSV, agrupamento de dados, ordenação e exportação de arrays. O projeto utiliza o Dash para criar uma interface gráfica interativa que permite visualizar os tempos de execução de cada biblioteca e métrica selecionada.

## Funcionalidades

- Leitura de dados de diferentes bibliotecas (`Pandas`, `Polars`, `Vaex`, `Datatable`).
- Comparação do tempo de execução para operações de:
  - Leitura (`read_time`)
  - Agrupamento (`group_time`)
  - Ordenação (`sort_time`)
  - Exportação (`offload_time`)
- Medição de uso de memória e pico de memória.
- Visualização dos resultados em um gráfico interativo utilizando `Dash` e `Plotly`.
- Filtro para selecionar a métrica de execução que deseja visualizar.

## Estrutura do Projeto

- `app.py`: Script principal que inicia a aplicação Dash e exibe os gráficos interativos.
- `metrics.py`: Contém as funções para realizar as medições de tempo de execução e memória das diferentes operações nas bibliotecas.
- `plot_memory_usage.py`: Contém a função para criar o gráfico de uso de memória comparando o uso de memória e o pico de memória para cada biblioteca.
- `requirements.txt`: Lista as dependências do projeto.

## Como Executar

### Pré-requisitos

- Python 3.7-3.11
- As bibliotecas necessárias estão listadas no arquivo `requirements.txt`. Você pode instalá-las usando o comando:

```bash
pip install -r requirements.txt
