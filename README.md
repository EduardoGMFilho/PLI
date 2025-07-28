
# 📊 Programação Linear Inteira com Python-MIP

Este repositório contém a implementação de dois problemas clássicos de **Programação Linear Inteira (PLI)** resolvidos com o pacote [`Python-MIP`](https://pypi.org/project/mip/). Os modelos são formulados para minimizar custos em cenários reais, como alocação de pessoal e corte de materiais.

## 🧩 Problemas Resolvidos

### 🧑‍💼 Problema 1: Alocação de Funcionários (Exercício 3.7 - Livro de Pesquisa Operacional)

**Descrição:**

Uma loja precisa alocar funcionários em tempo integral para cada dia da semana, conforme a tabela de demanda diária:

| Dia       | Funcionários necessários |
|-----------|---------------------------|
| Segunda   | 10                        |
| Terça     | 6                         |
| Quarta    | 8                         |
| Quinta    | 5                         |
| Sexta     | 9                         |
| Sábado    | 4                         |
| Domingo   | 6                         |

Cada funcionário trabalha **5 dias consecutivos** e folga 2, recebendo **R$30 por dia**. O objetivo é minimizar o custo total com salários, respeitando a demanda diária.

**Modelagem:**
- Variáveis inteiras representam o número de funcionários contratados em cada dia.
- Restrições garantem a cobertura da demanda com base nos ciclos de trabalho de 5 dias.
- Função objetivo: minimizar o número total de funcionários (proporcional ao custo total).

**Resultado ótimo:**
- Custo mínimo com 11 funcionários.

---

### 🔧 Problema 2: Otimização de Corte de Barras (Lista Prof. Marcone - UFOP)

**Descrição:**

Uma serralheria dispõe de barras de **6 metros** que devem ser cortadas nos seguintes comprimentos:

- 50 barras de 2m  
- 60 barras de 3m  
- 90 barras de 4m  

**Objetivo:** Minimizar o número total de barras de 6m utilizadas, considerando combinações viáveis de corte.

**Combinações modeladas:**
- 3 barras de 2m  
- 2 barras de 3m  
- 1 barra de 4m + 1 barra de 2m  
- 1 barra de 3m + 1 barra de 2m  

**Resultado ótimo:**
- Total de 120 barras de 6m utilizadas.

---

## 🧠 Competências Desenvolvidas

Durante a resolução dos problemas, foram aplicadas e aprimoradas as seguintes competências:

- **Modelagem matemática de problemas reais usando variáveis inteiras**
- **Formulação de funções objetivo e restrições lineares**
- **Utilização da biblioteca `mip` para construção e resolução de modelos PLI**
- **Interpretação de soluções ótimas e análise de sensibilidade**
- **Automatização de testes com funções auxiliares de resolução e salvamento**
- **Raciocínio lógico e otimização de recursos em contextos operacionais**

---

## 🛠️ Tecnologias e Ferramentas

- **Linguagem:** Python 3  
- **Biblioteca:** [Python-MIP (`mip`)](https://pypi.org/project/mip/)  
- **Solver:** CBC (Coin-or Branch and Cut)



Referências: https://sites.google.com/view/po-ufpb/in%C3%ADcio?authuser=0
