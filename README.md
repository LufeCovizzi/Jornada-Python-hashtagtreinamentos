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
