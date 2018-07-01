# Docesfinge

## objetivos
* Apresentar o formato RST do Sphinx de uma maneira dócil e sociável.

## Roteiro
1. Criar um arquivo para si: `touch estudante/${USER}.rst
2. Verificar a criação do arquivo do passo anterior: `ls estudante/`
3. Criar um arquivo para cidade onde você mora: `touch cidade/<nome-cidade>.rst`
4. Verificar a criação do arquivo do passo anterior: `ls cidade/`
5. Editar o arquivo de seu usuário seguindo o [modelo](#mod-arq-usuario): `\<EDITOR> estudante/${USER}.rst
6. Editar o arquivo de sua cidade seguindo o [modelo](#mod-arq-cidade): `\<EDITOR> cidade/<nome-cidade>.rst
7. Gerar documentação no formato HTML: `make html`
8. Visualizar os arquivos HTML gerados: `(cd _build/html; ls)`

<a name="mod-arq-usuario">

## Modelo para arquivo `<nome>.<sobrenome>.rst`

```rst
.. _<nome>.<sobrenome>:

<Nome> <Sobrenome>
==================

Quem sou
--------
Meu nome é <Nome> <Sobrenome>, 
moro da cidade de :ref:`<sigla-cidade>`, 
no bairro :ref:`<sigla-cidade>-<Nome do bairro1>` 

[...]

O que gosto de fazer
--------------------


O que sei fazer bem
-------------------
```

<a name="mod-arq-cidade">

## Modelo para arquivo `<nome-cidade>.rst`

```rst

.. _<sigla-cidade>:

<Nome da cidade>
================

.. _<sigla-cidade>-<Nome do bairro1>:

<Nome do bairro1>
=================

Moradores do bairro:
  * :ref:`<nome1>.<sobrenome1>`
  * :ref:`<nome2>.<sobrenome2>`

.. _<sigla-cidade>-<Nome do bairro2>:

<Nome do bairro2>
=================

[...]

.. _<sigla-cidade>-<Nome do bairroN>:

<Nome do bairroN>
=================
 
  
```
