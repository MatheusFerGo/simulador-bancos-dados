# 🎲 Laboratório de Arquitetura de Bancos de Dados

Um repositório prático e modular construído em Python (Jupyter Notebooks) para testar, visualizar e comparar a performance dos cinco principais tipos de bancos de dados do mercado sob estresse de milhões de registros.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![SQL](https://img.shields.io/badge/SQL-B--Tree_Indexes-blue.svg)
![NoSQL](https://img.shields.io/badge/NoSQL-Document_Stores-green.svg)
![Redis](https://img.shields.io/badge/Key--Value-O(1)_Lookup-red.svg)
![Graphs](https://img.shields.io/badge/Graphs-Index_Free_Adjacency-orange.svg)
![TimeSeries](https://img.shields.io/badge/Time_Series-Window_Slicing-purple.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Learning_Lab-orange.svg)

---

## 💡 Objetivo do Projeto

A teoria sobre qual banco de dados utilizar pode parecer abstrata. Este laboratório transforma conceitos arquiteturais em experimentos práticos.

Para cada tecnologia (SQL, Documentos, Chave-Valor, Grafos e Séries Temporais), o sistema gera automaticamente uma massa de dados local simulando cenários reais com milhões de registros. Em seguida, uma interface interativa permite comparar uma **consulta arquiteturalmente eficiente** contra uma **consulta ineficiente**, demonstrando o impacto direto na performance, tempo de resposta e volume de processamento.

---

## 📂 Estrutura do Repositório

```text
📁 simulador-bancos-dados
│
├── 📄 README.md
├── 📄 requirements.txt
│
├── 📁 1_Relacional_SQL
│   ├── 📓 simulador_sql.ipynb
│   └── 🗄️ banco_clientes.db
│
├── 📁 2_Documentos_NoSQL
│   ├── 📓 simulador_docs.ipynb
│   └── 📄 catalogo_produtos.json
│
├── 📁 3_Chave_Valor
│   ├── 📓 simulador_redis.ipynb
│   └── 📄 cache_sessoes.json
│
├── 📁 4_Grafos
│   ├── 📓 simulador_grafos.ipynb
│   └── 📊 conexoes_sociais.csv
│
└── 📁 5_Series_Temporais
    ├── 📓 simulador_ts.ipynb
    └── 📈 telemetria_servidor.csv
```

---

## 🔬 O que é testado em cada módulo?

### 🏛️ Banco de Dados Relacional (SQL)
- Busca por chave primária utilizando índice B-Tree.
- Comparação com Full Table Scan.
- Estudo de índices e otimização de consultas.

### 📄 Banco de Dados de Documentos (NoSQL)
- Busca direta por identificador.
- Consultas em propriedades JSON não indexadas.

### 🔑 Banco de Dados Chave-Valor
- Acesso O(1) por chave.
- Comparação com varredura linear O(N).

### 🕸️ Banco de Dados Orientado a Grafos
- Navegação entre nós conectados.
- Processamento global da rede.

### 📈 Banco de Dados de Séries Temporais
- Consultas por janela temporal.
- Comparação com filtros em massa.

---

## 🚀 Como Executar o Projeto

### Clone o repositório

```bash
git clone https://github.com/SEU_USUARIO/simulador-bancos-dados.git
cd simulador-bancos-dados
```

### Instale as dependências

```bash
pip install -r requirements.txt
```

### Inicie o Jupyter

```bash
jupyter notebook
```

---


Desenvolvido como projeto de estudo e demonstração prática de conceitos