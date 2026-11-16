# Teste — Implementação de uma Rede Neural

**Disciplina:** Matemática Computacional  
**Professor:** Prof. Dr. Alexsandro O. A.

## Sobre o projeto

Este projeto consiste na implementação da propagação direta (*forward pass*) de uma rede neural previamente treinada, utilizando Python e NumPy.

O objetivo é receber os dados de uma entrega, realizar a normalização dos atributos e utilizar os pesos e vieses fornecidos para prever a modalidade de envio mais adequada.

## Tecnologias utilizadas

- Python
- NumPy
- Pandas

## Arquitetura da rede neural

A rede possui a seguinte topologia:

**4 → 6 → 4 → 3**

- Camada de entrada: 4 neurônios.
- Primeira camada oculta: 6 neurônios, com ativação ReLU.
- Segunda camada oculta: 4 neurônios, com ativação tanh.
- Camada de saída: 3 neurônios, com ativação softmax.

As classes de saída são:
- PAC
- SEDEX
- SEDEX 10

## Funcionalidades implementadas

- Normalização dos atributos de entrada.
- Função de ativação ReLU.
- Função de ativação tanh.
- Função de ativação softmax.
- Multiplicação de matrizes por vetores.
- Propagação direta pelas três camadas.
- Classificação da modalidade de entrega.
- Validação dos resultados com o exemplo fornecido pelo professor.
- Avaliação das 10 entregas do arquivo CSV.

## Estrutura dos arquivos

```text
teste-rede-neural/
├── README.md
├── rede_template.py
├── pesos_rede.json
└── entregas_teste_rede.csv
```

## Como executar

1. Instale as dependências:

```bash
pip install numpy pandas
```

2. Coloque os três arquivos do projeto na mesma pasta.

3. Execute o programa:

```bash
python rede_template.py
```

## Resultados

A implementação passou pelas seis etapas do teste de validação fornecido pelo professor.

- Total de parâmetros: 73.
- Validação da propagação direta: aprovada.
- Acurácia nas 10 entregas de teste: 80% (8 acertos).

## Observação

Os pesos e vieses utilizados são os fornecidos pelo professor no arquivo `pesos_rede.json`. O projeto implementa somente a propagação direta, sem realizar treinamento ou ajuste dos parâmetros da rede.
