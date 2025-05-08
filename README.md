# 📇 Leitor de Contatos CSV

Este projeto é uma aplicação simples desenvolvida em Python para leitura e busca de contatos armazenados em um arquivo CSV. O objetivo é permitir que o usuário pesquise informações específicas como nome, email ou telefone, de maneira prática e interativa via terminal.

## 🚀 Funcionalidades

* Leitura automática de um arquivo `contato.csv`.
* Armazenamento dos contatos em uma lista de dicionários.
* Busca interativa por:

  * Nome
  * Email
  * Telefone
* Interface em linha de comando (CLI).
* Repetição de pesquisas até que o usuário decida sair.

## 🛠️ Tecnologias Utilizadas

* **Python 3**
* **Módulo CSV (padrão da linguagem)**

## 📂 Estrutura Esperada do Arquivo `contato.csv`

O arquivo `contato.csv` deve estar no mesmo diretório do script e conter um cabeçalho com os seguintes campos (nomes exatos):

```
nome,email,telefone
```

Exemplo de conteúdo do arquivo:

```csv
nome,email,telefone
João Silva,joao@email.com,11999999999
Maria Oliveira,maria@email.com,11988888888
Carlos Souza,carlos@email.com,11977777777
```

## ⚙️ Como Executar o Projeto

1. Certifique-se de ter o Python 3 instalado na sua máquina.

2. Crie ou coloque um arquivo `contato.csv` com os dados conforme o exemplo acima.

3. Execute o script Python no terminal:

```bash
python projetos.py
```

4. Siga as instruções no terminal para buscar contatos por nome, email ou telefone.

## 📌 Exemplo de Uso

```
Digite a opção que deseja: 
1 - Para pesquisar por nome
2 - Para pesquisar por email
3 - Para pesquisar por telefone
1
Digite o nome que deseja pesquisar: João
[{'nome': 'João Silva', 'email': 'joao@email.com', 'telefone': '11999999999'}]
Deseja continuar? (s/n)
s
...
```

## 🔍 Como Funciona

1. O script abre e lê o arquivo `contato.csv` usando `csv.DictReader`, transformando cada linha em um dicionário Python.
2. Os dados são armazenados em uma lista chamada `contatos`.
3. O usuário interage via terminal e escolhe um dos campos para buscar.
4. O programa busca por qualquer ocorrência do termo informado (case-insensitive) no campo correspondente.
5. O usuário pode repetir o processo quantas vezes quiser.

## 🧠 Melhorias Futuras (Sugestões)

* Interface gráfica (GUI) com Tkinter ou PyQt.
* Validação de entrada do usuário.
* Inclusão de opção para adicionar, editar ou excluir contatos.
* Exportação de resultados para um novo arquivo CSV.

---

