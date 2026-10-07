# Diagrama Entidade-Relacionamento – Livraria

### Professora Ellen Martins Lopes da Silva - 03/09/2026

## 📚 Sobre o Projeto

Este projeto apresenta um **Diagrama Entidade-Relacionamento (DER)** que representa um sistema envolvendo clientes, pedidos, livros e livrarias.

O objetivo é demonstrar como essas entidades se relacionam e quais informações são armazenadas sobre cada uma delas, facilitando a compreensão da estrutura de um banco de dados.

## 🎯 Objetivos

* Identificar as entidades de um sistema.
* Definir os atributos de cada entidade.
* Representar os relacionamentos entre as entidades.
* Compreender as cardinalidades dos relacionamentos.
* Organizar as informações para auxiliar na modelagem de um banco de dados.

## 🗂️ Entidades e Atributos

### 1. Cliente

Representa as pessoas que realizam pedidos no sistema.

**Atributos:**

* `Id_cliente`
* `Nome`
* `CPF`
* `Cartão`

### 2. Pedido

Representa os pedidos realizados pelos clientes.

**Atributos:**

* `Id-pedido`
* `Rastreamento`
* `Pagamento`
* `Prazo entrega`

### 3. Livro

Representa os livros disponíveis no sistema.

**Atributos:**

* `Id_livro`
* `Gênero`
* `Preço`
* `Autor`

### 4. Livraria

Representa a livraria relacionada aos livros.

**Atributos:**

* `Sistema`
* `Contato`
* `Requisição`
* `CNPJ`

## 🔗 Relacionamentos

### 1. Cliente – Faz – Pedido

Representa a realização de pedidos pelos clientes.

De acordo com as cardinalidades apresentadas no diagrama:

* Um cliente pode realizar um ou vários pedidos.
* Cada pedido está relacionado a um único cliente.

### 2. Pedido – Contém – Livro

Representa os livros que fazem parte de um pedido.

De acordo com o diagrama:

* Um pedido contém um ou vários livros.
* Um livro pode estar relacionado a um ou vários pedidos.

### 3. Livraria – Fornece – Livro

Representa o fornecimento de livros pela livraria.

Conforme as cardinalidades indicadas:

* Uma livraria pode fornecer um ou vários livros.
* Cada livro está relacionado a uma única livraria nesse relacionamento.

### 4. Livraria – Está na – Livro

O diagrama também apresenta o relacionamento **Está na**, conectando as entidades Livraria e Livro.

As cardinalidades indicadas representam uma relação de um para muitos, conforme a participação de cada entidade no diagrama.

## 🔢 Cardinalidade

A cardinalidade indica quantas ocorrências de uma entidade podem estar relacionadas a outra.

No diagrama, são utilizadas as seguintes indicações:

* **(1,1):** representa exatamente uma ocorrência.
* **(1,n):** representa uma ou várias ocorrências.

Essas informações ajudam a compreender as regras dos relacionamentos e a estruturar corretamente o banco de dados.

## 🛠️ Modelagem do Banco de Dados

O Diagrama Entidade-Relacionamento permite visualizar a estrutura do sistema antes da criação das tabelas no banco de dados.

A partir dele, é possível identificar as entidades, seus atributos e os relacionamentos que deverão ser considerados durante a implementação.

Os atributos identificadores, como `Id_cliente`, `Id-pedido` e `Id_livro`, ajudam a distinguir os registros de cada entidade.

## ✅ Considerações Finais

A construção do DER é uma etapa importante na modelagem de banco de dados, pois permite organizar as informações e compreender como elas se relacionam.

Neste diagrama, as entidades Cliente, Pedido, Livro e Livraria representam os principais elementos do sistema. Seus atributos e relacionamentos servem como base para o desenvolvimento de uma estrutura de banco de dados organizada.
