# Associando Conceitos IA, ML e Visão Computacional com Lógica de Programação

![Segmento](https://img.shields.io/badge/Segmento_:-IA-blue?style=flat-square)
![Tecnologias](https://img.shields.io/badge/Tecnologias_:-AzureMachineLearning-lightyellow?style=flat-square) 
![Ano](https://img.shields.io/badge/Ano_:-2025-darkyellow?style=flat-square)

Esta é a minha resposta ao primeiro desafio propostro curso Microsoft - Fundamentos de IA oferecido pela DIO.

## Objetivo

Associar corretamente cada conceito de IA com sua descrição correspondente, aprofundando seu entendimento sobre os princípios básicos dessa tecnologia.

## Estrutura

* **Entrada**

 Você receberá um conceito relacionado à IA e deverá fornecer a descrição correspondente. Os conceitos válidos para este desafio são:

* "processamento de linguagem natural"
* "machine learning"
* "visão computacional"
* "ia generativa"

* **Saída**

  Descrição associada ao conceito fornecido como entrada.

* "gera novos resultados a partir de dados existentes"
* "capacidade da IA para interpretar e entender o mundo visual"
* "habilidades de IA para entender e gerar linguagem humana"
* "permite que sistemas aprendam e melhorem a partir de dados"

## Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas.

**Entrada	Saída**

| Entrada                              | Saída             |
|--------------------------------------|----------------------------------------------------------------|
| processamento de linguagem natural   | habilidades de IA para entender e gerar linguagem humana       |
| machine learning	                   | permite que sistemas aprendam e melhorem a partir de dados     |
| visão computacional	                 | capacidade da IA para interpretar e entender o mundo visual    |

## O Código em Pyhton 

Abaixo está o código criado em resposta, em linguagem python.

   ```bash
# Recebe a Entrada do usuário e armazena na variável "entrada"
entrada = input()

# Função responsável por receber um conceito e retornar sua respectiva descrição.
def descrever_conceito(conceito):
    if conceito == "processamento de linguagem natural":
        return "habilidades de IA para entender e gerar linguagem humana"
    
    # COMPLETE AQUI: Preencha corretamente cada conceito, considerando as descrições abaixo:                         
    elif conceito == "visão computacional":
        return "capacidade da IA para interpretar e entender o mundo visual"
        
    elif conceito == "ia generativa":
        return "gera novos resultados a partir de dados existentes"
        
    elif conceito == "machine learning":
        return "permite que sistemas aprendam e melhorem a partir de dados"

# Imprime a descrição do conceito recebido na "entrada" através da função "descrever_conceito".  
print(descrever_conceito(entrada))
    main()
   ```
