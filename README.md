# Jornada Python - Hashtag Treinamentos

Repositório com os projetos da Jornada Python, da Hashtag Treinamentos. O foco das aulas é **automação de tarefas com Python**, usando bibliotecas como `pyautogui` e `pandas`.

## Aula 1 - Automação de cadastro de produtos

Script que automatiza o login em um sistema web e o cadastro de produtos a partir de uma planilha, simulando cliques e digitação como um usuário faria manualmente.

- [Aula1.py](Aula%201/Aula1.py): abre o navegador, faz login no sistema e cadastra, um a um, os produtos listados em `produtos.csv`.
- [pegar_posicao.py](Aula%201/pegar_posicao.py): utilitário para descobrir a posição (x, y) do cursor na tela, usado para mapear onde clicar durante a automação.
- [produtos.csv](Aula%201/produtos.csv): base de produtos (código, marca, tipo, categoria, preço, custo, observações) usada como fonte de dados do cadastro.

### Bibliotecas utilizadas

- [`pyautogui`](https://pyautogui.readthedocs.io/): controle automatizado de mouse e teclado.
- [`pandas`](https://pandas.pydata.org/): leitura e manipulação da base de produtos (CSV).

### Como executar

```bash
pip install pyautogui pandas
python "Aula 1/Aula1.py"
```

> Antes de rodar, ajuste as coordenadas de clique e as credenciais de login no script conforme o seu ambiente.

## Aula 2 - Analisando dados com Python (Python Insights)

Case de uma empresa com mais de 800 mil clientes que precisa entender os principais motivos de cancelamento do serviço. O notebook trata a base de dados, analisa a taxa de cancelamento e cruza cada coluna com o cancelamento para identificar os fatores de maior impacto.

- [Aula2.ipynb](Aula%202/Aula2.ipynb): gabarito original passado pelo professor durante a aula (saídas/gráficos removidos para manter o arquivo leve - basta rodar as células novamente).
- [aula2_codigo_final.ipynb](Aula%202/aula2_codigo_final.ipynb): versão reorganizada do mesmo código, com o passo a passo da análise - importação e tratamento da base, análise da taxa de cancelamento, geração de gráficos por coluna e filtragem dos clientes segundo os fatores identificados.
- [cancelamentos.csv](Aula%202/cancelamentos.csv): base de dados de clientes (contrato, forma de pagamento, dias de atraso, ligações ao call center, cancelou ou não, entre outras colunas) usada na análise.

> O `Aula2.ipynb` lê o arquivo como `cancelamentos_sample.csv` (nome usado originalmente pelo professor). Renomeie `cancelamentos.csv` ou ajuste essa linha antes de rodar esse notebook.

### Bibliotecas utilizadas

- [`pandas`](https://pandas.pydata.org/): leitura e tratamento da base de dados (CSV).
- [`plotly`](https://plotly.com/python/): geração dos gráficos de análise.

### Como executar

```bash
pip install pandas plotly openpyxl nbformat ipykernel
jupyter notebook "Aula 2/aula2_codigo_final.ipynb"
```
