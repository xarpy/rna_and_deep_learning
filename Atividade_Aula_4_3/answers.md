# Relatório Técnico: Atividade Aula 4.3
**Disciplina:** Redes Neurais / Deep Learning
**Dataset Utilizado:** Spiral (TensorFlow Playground)

---

## 1. Captura de Tela da Solução
[Insira aqui a screenshot do seu TensorFlow Playground com a espiral perfeitamente classificada]

---

## 2. Análise dos Parâmetros e Aprendizados

### A. Número de Camadas e Neurônios por Camada
* **O que foi observado:** Para padrões altamente não-lineares como a espiral, redes rasas (com poucas camadas) falham em criar as curvaturas complexas necessárias. Cada camada adicional permite que a rede combine características anteriores para formar fronteiras de decisão mais complexas. Neurônios extras em cada camada aumentam a quantidade de "linhas de corte" que podem ser combinadas.

### B. Tipo de Ativação
* **O que foi observado:** Funções de ativação lineares tornam a rede incapaz de resolver a espiral, independentemente de quantas camadas ela possua. A `ReLU` e a `Tanh` introduzem a não-linearidade necessária. A `ReLU` costuma convergir de forma mais rápida devido ao comportamento dos seus gradientes, enquanto funções como a `Sigmoid` podem sofrer com o desaparecimento do gradiente em redes profundas.

### C. Taxa de Aprendizado (Learning Rate)
* **O que foi observado:** Se a taxa for muito alta (ex: `3.0` ou `10.0`), os pesos divergem e a perda oscila agressivamente sem nunca classificar a espiral. Se for muito baixa (ex: `0.0001`), o treinamento se torna extremamente lento, podendo ficar preso em mínimos locais. Uma taxa intermediária (como `0.03` ou `0.1`) apresenta o melhor equilíbrio de convergência.

### D. Fator de Regularização (L1 / L2)
* **O que foi observado:** A regularização ajuda a simplificar os pesos da rede. No caso da espiral, se o fator de regularização for muito alto, a rede prioriza manter os pesos baixos em vez de aprender a forma complexa, gerando *underfitting*. Ajustada corretamente, ela suaviza as fronteiras de decisão, evitando ruídos desnecessários (ruído de *overfitting*).