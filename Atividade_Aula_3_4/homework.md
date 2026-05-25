# Atividade Aula 3.4

Utilizando como base o código `3.4-LogisticRegressionMNIST-SGD.ipynb`, responda às perguntas e realize as atividades abaixo. Para submissão, submeta sua resposta no repositório criado para a disciplina.

> **Observação:** Coloque o resultado dentro de uma pasta chamada **"Atividade Aula 3.4"**.

---

### Perguntas Teóricas

1. Qual é o tamanho do mini-batch?
2. Em uma época, quantos mini-batches existem?
3. Qual é a definição de época?

---

### Exercícios Práticos

### 1. Monitoramento de Batches
Coloque um print no final de cada mini-batch, seguindo o mesmo padrão do print de fim de época. Utilize o formato abaixo:
* `Época: 1/4, batch: 600`

### 2. Análise de Hiperparâmetros (Batch Size)
Altere o tamanho do mini-batch (`batch_size`) algumas vezes, refaça o treinamento e compare em um gráfico a queda da perda para cada tamanho de mini-batch testado.