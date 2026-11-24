# Chamados ADS

Este repositório é utilizado apenas como resposta as atividades da disciplina de Programação para Web do curso de ADS, da UFCA.

## 1. Nome completo do estudante.
Lucas do Nascimento Souza<br>
2023011395

## 2. Objetivo do projeto.
Este projeto tem como objetivo aplicar na prática os conceitos aprendidos em aula sobre como desenvolver um simples sistema de backend usando python com o framework flask.

## 3. Como instalar as dependências com uv sync --locked.
Estas etapas é opcional, mas recomendada.
### 3.1. Criando o Ambiente Virtual (`.venv`)
Antes de instalar as dependências, é recomendado isolar o ambiente do projeto. Na raiz do diretório (`chamados-ads`), crie o ambiente virtual utilizando o `uv` (que identificará automaticamente a exigência do **Python 3.14+** definida no `pyproject.toml`):

```
uv venv
```
(Caso prefira utilizar o módulo nativo do Python, execute ```python -m venv .venv```.)
### 3.2. Ativando o Ambiente Virtual
- Linux / macOS:
  ```
  source .venv/bin/activate
  ```
- Windows (PowerShell):
  ```
  .venv\Scripts\Activate.ps1
  ```
- Windows (Prompt de Comando / CMD):
  ```
  .venv\Scripts\activate.bat
  ```
(Quando ativado com sucesso, o nome (.venv) aparecerá no início da linha do seu terminal.)

O projeto utiliza o gerenciador de pacotes `uv` e exige **Python 3.14** ou superior. Para criar o ambiente virtual e instalar as dependências exatamente conforme definidas no arquivo `uv.lock`, execute o comando abaixo na raiz do projeto:

```
uv sync --locked
```
O próprio comando ```uv sync --locked``` também é capaz de criar a pasta .venv automaticamente caso ela ainda não exista, mas seguir os passos 3.1 e 3.2 garante que o terminal já esteja apontando para o interpretador isolado correto.

## 4. Como executar a aplicação.
Com as dependências instaladas, inicie o servidor local do Flask utilizando o ambiente gerenciado pelo uv.

```
uv run flask run
```

(Caso já tenha ativado o ambiente virtual .venv manualmente, você pode executar diretamente ```flask run```.)

Por padrão, a aplicação será iniciada no endereço http://127.0.0.1:5000

## 5. Como acessar a rota inicial e qual resposta esperar.
Acesso à Rota Inicial e Resposta Esperada
Para testar se a aplicação está operando corretamente, acesse a rota raiz (GET /) através do seu navegador, Postman/Insomnia ou via terminal com curl:

```curl``` [http://127.0.0.1:5000/](http://127.0.0.1:5000/)
