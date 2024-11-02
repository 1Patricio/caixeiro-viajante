# Algoritmo Genético para o Problema do Caixeiro Viajante

Este repositório contém uma implementação de um algoritmo genético para resolver o problema do caixeiro viajante (TSP) utilizando JavaScript. O objetivo do algoritmo é encontrar o caminho mais curto possível que passe por todas as cidades e retorne à cidade inicial, minimizando a distância total percorrida.

## Tabela de Conteúdos

- [Visão Geral](#visão-geral)
- [Como Funciona](#como-funciona)
- [Instalação](#instalação)
- [Uso](#uso)
- [Contribuição](#contribuição)

## Visão Geral

O algoritmo genético simula o processo da seleção natural, onde soluções (caminhos) são geradas, avaliadas, selecionadas e combinadas para criar novas soluções. A implementação segue as seguintes etapas:

1. **Geração Inicial**: Criação de uma população inicial de caminhos aleatórios.
2. **Avaliação**: Cálculo da aptidão de cada caminho (inverso da distância total).
3. **Seleção**: Seleção dos melhores caminhos para reprodução.
4. **Cruzamento**: Combinação de dois caminhos para criar novos caminhos.
5. **Mutação**: Introdução de pequenas alterações nos novos caminhos.
6. **Repetição**: O processo é repetido por várias gerações até atingir um critério de parada.

## Como Funciona

O código principal está estruturado nas seguintes funções:

- **calculoDistanciaEntrePontos(cidadeA, cidadeB)**: Calcula a distância entre duas cidades usando a fórmula da distância euclidiana.
- **calcularDistanciaTotal(rotaAtual)**: Calcula a distância total de uma rota.
- **gerarCaminhoAleatorio()**: Gera um caminho aleatório (indivíduo).
- **criargrupoCaminhos(tamanho)**: Cria uma nova população inicial de rotas.
- **aptidao(rotaAtual)**: Avalia a aptidão de uma rota.
- **escolherMelhoresCaminhos(grupoCaminhos)**: Seleciona os melhores caminhos para cruzamento.
- **cruzarCaminhos(rota1, rota2)**: Realiza o cruzamento entre dois caminhos.
- **mutacao(rotaAtual)**: Aplica mutação em um caminho.
- **algoritmoGenetico()**: Função principal que executa o algoritmo genético.

## Instalação

Para executar o projeto localmente, você precisa ter o Node.js instalado. Clone o repositório e navegue até a pasta do projeto:

```bash
git clone https://github.com/1Patricio/caixeiro-viajante.git
```

## Uso

Para rodar o algoritmo, utilize o seguinte comando:
``` bash
node caixeiro-viajante.js
```

## Contribuição 
Sinta-se à vontade para contribuir para este projeto. Você pode:

- Reportar problemas
- Sugerir melhorias
- Enviar pull requests