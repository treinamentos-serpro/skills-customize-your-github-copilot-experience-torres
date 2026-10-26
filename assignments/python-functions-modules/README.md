# 📘 Assignment: Python Functions and Modules

## 🎯 Objective

Organize um pequeno programa em funções reutilizáveis e módulos Python. Você praticará separar responsabilidades, importar funções e compor um programa a partir de arquivos distintos.

## 📝 Tasks

### 🛠️ Criar funções reutilizáveis

#### Descrição
Crie um programa simples para resumir uma lista de despesas. Comece organizando as operações em funções pequenas, cada uma com uma responsabilidade clara.

#### Requisitos
O programa concluído deve:

- Definir `calculate_total(amounts)` para retornar a soma dos valores
- Definir `calculate_average(amounts)` para retornar a média dos valores
- Retornar `0` como média quando a lista estiver vazia
- Demonstrar as funções com uma lista de valores, como `[12.5, 8.0, 9.5]`


### 🛠️ Separar funções em módulos

#### Descrição
Separe as funções de cálculo do ponto de entrada do programa para que possam ser importadas e reutilizadas.

#### Requisitos
O programa concluído deve:

- Criar `calculations.py` com `calculate_total()` e `calculate_average()`
- Criar `main.py` e importar as funções de `calculations.py`
- Executar os cálculos a partir de `main.py`, sem duplicar as funções nesse arquivo


### 🛠️ Montar um resumo com funções importadas

#### Descrição
Amplie o programa para formatar os valores e exibir um resumo legível das despesas, mantendo os cálculos e a formatação em módulos separados.

#### Requisitos
O programa concluído deve:

- Criar `formatting.py` com uma função `format_currency(amount)` que retorna o valor formatado como moeda
- Importar as funções de cálculo e formatação em `main.py`
- Exibir o total e a média das despesas usando as funções importadas
- Manter o ponto de entrada em `main.py`, sem duplicar lógica de cálculo ou formatação