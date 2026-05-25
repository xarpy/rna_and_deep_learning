# Atividade Aula 3.3

Utilizando como base o código `3.3-datasets-e-dataloaders.ipynb`, faça as atividades abaixo. Para submissão, submeta sua resposta no repositório criado para a disciplina.

> **Observação:** Coloque o resultado dentro de uma pasta chamada **"Atividade Aula 3.3"**.

---

### 1. Customização do DataLoader

* Defina seu próprio `DataLoader` na segunda célula indicada no notebook.
* Faça com que cada batch tenha **5 elementos** cada, utilizando o dataset já criado anteriormente.
* Em seguida, imprima o tamanho do `DataLoader` e o tamanho do `Dataset`.

---

### Questões Analíticas

* **Análise 1:** A ordem dos elementos se altera entre execuções da célula acima?
* **Análise 2:** Tente colocar o parâmetro `shuffle` do `DataLoader` como `True` e observe o resultado do exercício, rodando a célula várias vezes. O que muda?