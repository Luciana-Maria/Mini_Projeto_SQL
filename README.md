## 📊 Projeto de Análise de Dados: Livraria DevSaber  

![Status](https://img.shields.io/badge/status-finalizado-green)  ![BigQuery](https://img.shields.io/badge/BigQuery-Dataset-blue)  ![SQL](https://img.shields.io/badge/SQL-Scripts-lightgrey)  ![Canva](https://img.shields.io/badge/Canva-Apresentação-purple)  

Este projeto foi desenvolvido como parte do **Programa Desenvolve Grupo Boticário 2025** e tem como objetivo a **criação e análise de dados** de uma loja fictícia chamada **Livraria DevSaber**.  

💡 A ideia foi montar um **dataset no BigQuery**, realizar **consultas de negócio** e criar uma **view analítica** para facilitar a exploração dos dados.  
A apresentação visual foi feita no **Canva**.  

---

## 🗂️ Estrutura do Projeto  

📁 Arquivos disponíveis no repositório:  
- `apresentacao_devsaber.pdf` → Slides da apresentação do projeto.  
- `consultas_sql.pdf` → Consultas de negócio realizadas no BigQuery.  
- `scripts_criacao_tabelas.pdf` → Scripts SQL para criação do esquema e tabelas.  

---

## 🚀 Passo a Passo  

### 1️⃣ Criação do Dataset  

```sql
CREATE SCHEMA t1engenhariadados.Turma_2_grupo15_Livraria_DevSaber
OPTIONS (
  description = "Conjunto de dados Livraria DevSaber",
  location = "US"
);
````

---

### 2️⃣ Estrutura das Tabelas

**📌 Clientes**

| Campo          | Tipo   |
| -------------- | ------ |
| id_cliente     | STRING |
| nome_cliente   | STRING |
| email_cliente  | STRING |
| cidade_cliente | STRING |
| estado_cliente | STRING |
| data_cadastro  | DATE   |

**📌 Produtos**

| Campo             | Tipo    |
| ----------------- | ------- |
| id_produto        | STRING  |
| titulo_produto    | STRING  |
| autor_produto     | STRING  |
| categoria_produto | STRING  |
| preco_produto     | NUMERIC |

**📌 Vendas**

| Campo             | Tipo      |
| ----------------- | --------- |
| id_venda          | STRING    |
| id_cliente        | STRING    |
| id_produto        | STRING    |
| data_venda        | TIMESTAMP |
| quantidade_venda  | INTEGER   |
| valor_total_venda | NUMERIC   |

---

### 3️⃣ Consultas de Negócio

Foram realizadas consultas SQL para responder perguntas de negócio, como:

* Total de produtos cadastrados.
* Preço médio dos livros.
* Produto mais caro e mais barato.
* Quantidade de produtos por categoria.
* Top 5 livros mais caros.

---

### 4️⃣ View Analítica

Criada a view **`freq_por_catProdutos`** para mostrar a **frequência de vendas por categoria**, ordenando do maior para o menor número de vendas.

---

## 🎨 Visualização

A apresentação do projeto foi criada no **Canva** e está disponível no arquivo `apresentacao_devsaber.pdf`.

---

## 🛠️ Tecnologias Utilizadas

* **Google BigQuery** → Armazenamento e análise dos dados
* **SQL** → Criação de tabelas e consultas de negócio
* **Canva** → Criação da apresentação visual

---

## 👩‍💻 Autoria

Projeto desenvolvido por **Luciana** durante o **Programa Desenvolve Grupo Boticário 2025**.

```
## 🔗 Conecte-se comigo

- [LinkedIn](https://linkedin.com/in/lucianaqa)

