# 🔢 Comparativo de Algoritmos de Ordenação  
**Disciplina:** Resolução de Problemas Estruturados em Computação  


---

## 🧩 Algoritmos Implementados

- **Comb Sort**  
- **Gnome Sort**  
- **Bucket Sort**  
- **Bubble Sort (com flag de parada)**  
- **Selection Sort**  
- **Cocktail Sort**

Nenhum algoritmo utiliza funções prontas da linguagem (como `Arrays.sort()`, `ArrayList` ou similares).  
Todos foram implementados utilizando apenas **estruturas básicas** (`for`, `while`, `if`, `int[]`).

---

## 📊 Tabelas de Resultados

### 🔹 Vetor 1 (Desordenado)
| Algoritmo      | Trocas | Iterações |
|----------------|--------|------------|
| Comb Sort      | 22     | 129        |
| Gnome Sort     | 78     | 175        |
| Bucket Sort    | 20     | 20         |
| Bubble Sort    | 78     | 180        |
| Selection Sort | 18     | 190        |
| Cocktail Sort  | 78     | 154        |

**Melhor em trocas:** Selection Sort  
**Melhor em iterações:** Bucket Sort  

---

### 🔹 Vetor 2 (Ordenado)
| Algoritmo      | Trocas | Iterações |
|----------------|--------|------------|
| Comb Sort      | 0      | 110        |
| Gnome Sort     | 0      | 19         |
| Bucket Sort    | 20     | 20         |
| Bubble Sort    | 0      | 19         |
| Selection Sort | 0      | 190        |
| Cocktail Sort  | 0      | 19         |

**Melhor em trocas:** Empate (Comb, Gnome, Bubble, Selection, Cocktail)  
**Melhor em iterações:** Gnome, Bubble e Cocktail Sort (19)  

---

### 🔹 Vetor 3 (Ordenado Decrescente)
| Algoritmo      | Trocas | Iterações |
|----------------|--------|------------|
| Comb Sort      | 18     | 129        |
| Gnome Sort     | 190    | 399        |
| Bucket Sort    | 20     | 20         |
| Bubble Sort    | 190    | 190        |
| Selection Sort | 10     | 190        |
| Cocktail Sort  | 190    | 190        |

**Melhor em trocas:** Selection Sort  
**Melhor em iterações:** Bucket Sort  

---

## 🏆 Rankings Gerais

### 🔸 Menos Trocas (média geral)
| Posição | Algoritmo      | Média de Trocas |
|----------|----------------|-----------------|
| 🥇 1º | **Selection Sort** | **9.33** |
| 🥈 2º | **Comb Sort**      | **13.33** |
| 🥉 3º | **Bucket Sort**    | **20.00** |
| 4º | Cocktail Sort         | 89.33 |
| 5º | Gnome Sort            | 89.33 |
| 6º | Bubble Sort           | 89.33 |

---

### 🔸 Menos Iterações (média geral)
| Posição | Algoritmo      | Média de Iterações |
|----------|----------------|--------------------|
| 🥇 1º | **Bucket Sort**    | **20.00** |
| 🥈 2º | **Gnome Sort**     | **197.66** |
| 🥉 3º | **Comb Sort**      | **122.66** |
| 4º | Cocktail Sort         | 121.00 |
| 5º | Bubble Sort           | 129.66 |
| 6º | Selection Sort        | 190.00 |

---

## 🧠 Conclusões

- **Bucket Sort** apresentou o **melhor desempenho em iterações** e excelente eficiência em vetores de tamanho controlado, pois sua contagem direta é quase linear.  
- **Selection Sort** foi o **mais econômico em trocas**, pois troca apenas uma vez por posição.  
- **Comb Sort** teve um bom equilíbrio entre trocas e iterações, sendo um avanço perceptível sobre o Bubble Sort.  
- **Gnome Sort**, **Bubble Sort** e **Cocktail Sort** tiveram desempenhos similares em vetores desordenados, exigindo muitas trocas e iterações.  
- Em vetores **já ordenados**, os algoritmos com verificação de flag (Bubble e Cocktail) e os com avanço adaptativo (Gnome) se destacaram, evitando processamento desnecessário.  
- Em vetores **decrescentes**, Selection Sort novamente se mostrou mais estável, realizando menos trocas mesmo com alto número de comparações.

---

