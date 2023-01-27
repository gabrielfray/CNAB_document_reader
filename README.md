# CNAB Document Reader

## Tabela de Conteúdos

1. [Sobre](#sobre)
2. [Techs](#techs)
3. [Instalação](#install)
4. [Como usar](#comousar)
5. [Desenvolvedores](#devs)
6. [Termos de uso](#terms)


---

<a name="sobre"></a>

## 1. Sobre

- O programa foi desenvolvido com o objetivo de processar arquivos CNAB, que contêm dados sobre movimentações financeiras de várias lojas. Ele armazena esses dados de forma organizada e de fácil leitura em um banco de dados relacional. 
- Para facilitar o uso do programa, foi criada uma interface web que permite o upload do arquivo CNAB. O arquivo é processado, os dados são normalizados e armazenados no banco de dados. As informações processadas podem ser visualizadas na tela.

<a name="techs"></a>

## 3. Techs

Visão Geral das tecnologias usadas no projeto.

- [Python](https://docs.python.org/3/)
- [Django](https://www.djangoproject.com/)
- [django rest_framework](https://www.django-rest-framework.org/)


---
<a align="left" name="techs"></a>

<a name="install"></a>

## 3. Instalação e uso

### 3.1 Requisitos

- Python a partir da versão 3.11.1
- Gerenciador de pacotes pip

### 3.2 Instalação

3.2.1 - Clone o repositório crie um ambiente de desenvolvimento:
 ```
 python -m venv venv
 ```
 
 3.2.2 - Após a criação do ambiente virtual voce terá que ativa-lo com o seguinte comando
 
 para linux:
 ```
 source/venv/bin/activate
 ```
 
 para windows:
 ```
 .\venv\Scripts\activate
 ```
 
 3.2.3 - Agora que ja ativou o ambiênte de desenvolvimento voce terá que instalar as dependências do projeto
```
pip install -r requirements.txt
```

3.2.4 - Após instalar as dependências vamos persistir as migrations no banco de dados
```
python manage.py migrate
```

3.2.5 Para rodar projeto utilize o comando 
```
python manage.py runserver
``` 

3.2.6 - Caso de tudo certo receberá uma mensagem parecida com essa:

```
System check identified no issues (0 silenced).
January 04, 2023 - 13:53:34
Django version 4.1.5, using settings 'djangoAnimes.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.
```

<a name="comousar"></a>

## 4. Como usar

- Para usar é bem simples, após o processo de instalção, 
