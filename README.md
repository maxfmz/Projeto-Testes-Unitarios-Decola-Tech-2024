## Desafio de projeto
Este é um desafio da trilha .NET da DIO, do bootcamp Decola Tech 2024 da Avanade.

## Contexto
Neste desafio, estou trabalhando em um sistema que anda tendo erros e bugs recorrentemente. Por conta disso, tive que implementar testes unitários em .NET, a fim de validar os processos e prevenir esses problemas.

## Premissas
**Classes e métodos de validação**

| Classe           | Método                       | Objetivo                                                                                                                
|------------------|------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ValidacoesLista | RemoverNumerosNegativos      | Recebe uma lista de números inteiros e retorna uma nova lista, apenas com os números positivos                                                              |
| ValidacoesLista | ListaContemDeterminadoNumero | Recebe uma lista de números inteiros e verifica se um determinado número está presente dentro dessa lista                                                   |
| ValidacoesLista | MultiplicarNumerosLista      | Recebe uma lista de números inteiros e retorna uma nova lista, com seus valores múltiplicados por um determinado número                                     |
| ValidacoesLista | RetornarMaiorNumeroLista     | Recebe uma lista de números inteiros e retorna o maior número entre eles                                                                                    |
| ValidacoesLista | RetornarMenorNumeroLista     | Recebe uma lista de números inteiros e retorna o menor número entre eles                                                                                    |
| ValidacoesString | RetornarQuantidadeCaracteres | Recebe um texto qualquer e retorna a quantidade de caracteres presentes no texto                                                                           |
| ValidacoesString | ContemCaractere              | Recebe um texto qualquer e um texto a ser procurado, retorna verdadeiro ou falso se um determinado trecho procurado está presente no texto                 |
| ValidacoesString | TextoTerminaCom              | Recebe um texto qualquer e um trecho a ser procurado, retorna verdadeiro ou falso se um determinado trecho procurado está presente no final do texto apenas |


**Classes e métodos de testes**

| Classe                | Método de teste                                  | Resultado esperado do teste
|---------------------- |--------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ValidacoesListaTests | DeveRemoverNumerosNegativosDeUmaLista         | Ao passar uma lista com diversos números, incluindo positivos e negativos, deve ser retornado uma nova lista apenas com números positivos                                                            |
| ValidacoesListaTests | DeveConterONumero9NaLista                     | Ao passar uma lista com diversos números, incluindo o número 9, deve retornar verdadeiro, pois encontrou o 9 na lista                                                                                |
| ValidacoesListaTests | NaoDeveConterONumero10NaLista                 | Ao passar uma lista com diversos números, mas sem o número 10, deve retornar falso, pois não encontrou o 10 na lista                                                                                 |
| ValidacoesListaTests | DeveMultiplicarOsElementosDaListaPor2         | Ao passar uma lista de inteiros, deve retornar uma nova lista, com todos os elementos da lista multiplicados por 2                                                                                   |
| ValidacoesListaTests | DeveRetornar9ComoMaiorNumeroDaLista           | Ao passar uma lista de números inteiros, sendo o maior deles 9, deve retornar o 9 como maior elemento dentro dessa lista                                                                             |
| ValidacoesListaTests | DeveRetornarOitoNegativoComoMenorNumeroDaList | Ao passar uma lista de números inteiros, sendo o menor deles -8, deve retornar o -8 como menor elemento dentro dessa lista                                                                           |
| ValidacoesStringTests | DeveRetornar6QuantidadeCaracteresDaPalavraMatrix | Ao passar um texto escrito a palavra "Matrix", deve retornar o número 6, representando 6 caracteres presentes na palavra                                                                         |
| ValidacoesStringTests | DeveContemAPalavraQualquerNoTexto                | Ao passar um texto escrito "Esse é um texto qualquer" e procurar pela palavra "qualquer", deve retornar verdadeiro pois a palavra existe no texto                                                |
| ValidacoesStringTests | NaoDeveConterAPalavraTesteNoTexto                | Ao passar um texto escrito "Esse é um texto qualquer" e procurar pela palavra "teste", deve retornar falso pois a palavra não existe no texto                                                    |
| ValidacoesStringTests | TextoDeveTerminarComAPalavraProcurado            | Ao passar um texto escrito "Começo, meio e fim do texto procurado" e procurar pela palavra "procurado", deve retornar verdadeiro pois a palavra existe no texto e está inclusa no final do texto |

## Estrutura do projeto

O projeto está estruturado da seguinte maneira:

![Métodos Swagger](Imagens/projeto.png)
