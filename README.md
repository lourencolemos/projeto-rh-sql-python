# 📊 Projeto RH - Análise de Dados com SQL e Python

## 👨‍🎓 Aluno

**Nome:** Lourenço Lemos

**Turma:** 2

---

# 🎯 Objetivo do Projeto

Este projeto tem como objetivo aplicar conceitos de SQL, Python e Análise Exploratória de Dados (EDA) utilizando a base de dados HR da Oracle.

Foram desenvolvidas consultas SQL para extração e relacionamento dos dados, seguidas de análises estatísticas e visualizações gráficas em Python, permitindo identificar padrões relacionados à distribuição salarial, departamentos e localização geográfica dos colaboradores.

---

# 🛠 Tecnologias Utilizadas

- Oracle SQL
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
- Git
- GitHub

---

# 📂 Estrutura do Projeto

```text
projeto-rh-sql-python/
│
├── data/
│   ├── raw_data/
│   └── processed_data/
│
├── sql/
│   ├── query_01.sql
│   └── query_02.sql
│
├── notebooks/
│   └── analise_rh.ipynb
│
├── images/
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# 🗄 Base de Dados

O projeto utiliza o esquema **HR (Human Resources)** da Oracle.

As principais tabelas utilizadas foram:

| Tabela | Descrição |
|---------|-----------|
| EMPLOYEES | Informações dos funcionários |
| JOBS | Cargos e faixas salariais |
| DEPARTMENTS | Departamentos |
| LOCATIONS | Localização dos departamentos |
| COUNTRIES | Países |
| REGIONS | Regiões geográficas |

---

# 🔍 Consulta SQL 01

### Objetivo

Relacionar funcionários, departamentos e cargos para realizar a análise da distribuição salarial.

### Informações obtidas

- Funcionário
- Salário
- Cargo
- Departamento
- Faixa salarial do cargo

---

# 📈 Análise da Query 01

Foram realizadas:

- Estatísticas descritivas
- Histograma da distribuição salarial
- Boxplot
- Salário médio por departamento
- Quantidade de funcionários por departamento

## Distribuição Salarial

![Histograma](images/query_01_histograma_salarios.png)

O histograma mostra concentração de colaboradores nas menores faixas salariais e poucos salários elevados, caracterizando uma distribuição assimétrica à direita.

---

## Boxplot

![Boxplot](images/query_01_boxplot_salarios.png)

O boxplot evidencia a presença de um outlier correspondente ao maior salário da empresa, pertencente a um cargo executivo.

---

## Salário Médio por Departamento

![Departamento](images/query_01_barplot_salario_departamento.png)

Os departamentos executivos apresentam maior remuneração média, enquanto áreas operacionais concentram salários menores.

---

## Quantidade de Funcionários

![Funcionários](images/query_01_barplot_funcionarios_departamento.png)

Os colaboradores concentram-se em poucos departamentos, enquanto áreas executivas possuem equipes reduzidas.

---

# 🌍 Consulta SQL 02

### Objetivo

Relacionar funcionários com departamentos, cidades, países e regiões para realizar uma análise geográfica da empresa.

### Informações obtidas

- Funcionário
- Salário
- Departamento
- Cidade
- País
- Região

---

# 📊 Análise da Query 02

Foram desenvolvidos gráficos para analisar:

- Funcionários por região
- Salário médio por região
- Funcionários por país
- Salário médio por país
- Top cidades com maior quantidade de funcionários

## Funcionários por Região

![Região](images/query_02_barplot_funcionarios_regiao.png)

A maior parte dos colaboradores concentra-se em uma única região geográfica.

---

## Salário Médio por Região

![Salário Região](images/query_02_barplot_salario_regiao.png)

Foram observadas diferenças salariais entre as regiões analisadas.

---

## Funcionários por País

![País](images/query_02_barplot_quantidade_funcionarios_pais.png)

Os Estados Unidos concentram a maior parte da força de trabalho da empresa.

---

## Salário Médio por País

![Salário País](images/query_02_barplot_salario_pais.png)

Os salários médios variam entre os países analisados, indicando diferenças na estrutura organizacional.

---

## Top Cidades

![Cidade](images/query_02_barplot_funcionarios_cidade.png)

As cidades com maior número de colaboradores representam os principais polos administrativos da empresa.

---

# 💡 Principais Resultados

A análise permitiu identificar que:

- A distribuição salarial é assimétrica.
- Poucos colaboradores concentram os maiores salários.
- Os departamentos executivos apresentam maior remuneração média.
- A maior parte dos funcionários está concentrada nos Estados Unidos.
- Existem diferenças salariais entre regiões e países.
- A estrutura da empresa apresenta características típicas de uma organização multinacional.

---

# ▶ Como Executar

1. Clone o repositório

```bash
git clone <URL_DO_REPOSITÓRIO>
```

2. Instale as dependências

```bash
pip install -r requirements.txt
```

3. Execute as consultas SQL na base HR Oracle.

4. Abra o notebook:

```text
notebooks/analise_rh.ipynb
```

5. Execute todas as células.

---

# 🚀 Melhorias Futuras

Como evolução deste projeto, podem ser implementadas as seguintes melhorias:

- Dashboard interativo em Power BI.
- Dashboard em Streamlit.
- Filtros dinâmicos.
- Comparação salarial por cargo.
- Análise temporal de admissões.
- Indicadores de Recursos Humanos (KPIs).
- Automatização da extração dos dados.

---

# 👤 Autor

**Lourenço Lemos**

Projeto desenvolvido como atividade prática da disciplina de Análise de Dados da SCTEC.
