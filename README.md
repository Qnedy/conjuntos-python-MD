
# Algoritmos de operação de conjuntos utilizando python

#### Alunos: Ezequiel, Kennedy, Taylor e Alexandre Matos

### Algoritmo 1: Intersecção(A, B)
>Entradas: A e B são conjuntos 
Saída: o conjunto resultante da intersecção


1. C $\leftarrow$ {&nbsp;} 
2. para cada $a \in$ $A$ faça
3. &nbsp;&nbsp; se $a \in B$ faça
4. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;$C$$\leftarrow a$
5. &nbsp;&nbsp; fim
6. fim
7. retorne $C$


Explicação:

O algoritmo interseccao demonstra como funcionaria um programa que faz a intersecção entre dois conjuntos. Como argumentos para o método têm-se duas variáveis ambas conjuntos numéricos. Na linha 1 é atribuído um conjunto vazio a C. Depois o primeiro conjunto passado como parâmetro (A) é percorrido e, a cada elemento deste, faz-se uma comparação onde o objetivo é verificar se o elemento atual em análise também é um elemento do segundo conjunto, também passado como parâmetro (B). Caso essa comparação retorne verdade, o elemento é atribuído ao conjunto - antes vazio - C. Por fim, o algoritmo retorna todo o conjunto C, onde os elementos contidos nele são os elementos que fazem intersecção entre os dois conjuntos analisados.

Código em python:

```python
def intersecao(lista1, lista2):  
	lista3 = {}  
	for n in lista1:  
		if n in lista2:  
			lista3.append(n)  
	return lista3
```




### Algoritmo 2: União(A, B)
>Entradas: A e B são conjuntos** 
Saída: o conjunto resultante da união
 Insere(&nbsp;): insere um elemento ao conjunto


1. C $\leftarrow$ {&nbsp;} 
2. para cada $a \in$ $A$ faça
3. &nbsp;&nbsp; Insere($C, a$)
4. fim
5. para cada $b \in$ $B$ faça
6. &nbsp;&nbsp; Insere($C, b$)
7. fim
8. retorne $C$

Explicação:

O algoritmo de união realiza a união entre dois conjuntos. Ele recebe como parâmetros dois conjuntos sob os quais a operação de união será realizada (A e B). Utilizando algumas iterações o conjunto A é percorrido, e cada um dos seus  elementos é adicionado a um conjunto resultante da união (&nbsp;C). O conjunto B recebido como parâmetro também é percorrido da mesma forma que o A foi, e, para cada elemento do conjunto B, é verificado se o elemento já existe no conjunto resultante (&nbsp;C), caso o elemento não exista, ele é adicionado a esse conjunto. Para finalizar a rotina, é retornado o conjunto resultante da união entre os dois conjuntos recebidos como parâmetros na função.

Código python:
```python
def uniao(A, B):  
	C = {}  
	for a in A:  
		C.append(a)  
	for e in B:  
		if e not in C:  
			C.append(e)  
	return C
```

### Algoritmo 3: Diferença(A, B)
>Entradas: A e B são conjuntos 
Saída: o conjunto resultante da diferença entre os conjuntos.

1. $C$ $\leftarrow$ {&nbsp;} 
2. para cada $a \in$ $A$ faça
3. &nbsp;&nbsp; se $a \notin B$ faça
4. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;$C$$\leftarrow a$
5. &nbsp;&nbsp; fim
6. fim
7. retorne $C$

Explicação:

O algoritmo diferenca retorna a diferença entre dois conjuntos. Ele recebe como parâmetro duas entradas que são conjuntos numéricos, A e B respectivamente. Na outra linha é atribuído um conjunto vazio a C (linha 1).O conjunto A é percorrido e cada elemento dele é comparado, onde o objetivo é descobrir se o elemento em questão não está em B. Caso retorne verdade, o elemento analisado naquele momento será acrescentado no final do conjunto C (ou início, caso seja o primeiro elemento do conjunto). Por fim o conjunto C é retornado, exibindo o conjunto diferença entre os conjuntos analisados.

Código em Python:
```python
def diferenca(A, B):
	C = []
	for a in A:
		if a not in B:
			B.append(a)
	return C
```

### Algoritmo 4: Plano cartesiano(A, B)
>Entradas: A e B são conjuntos
Saída: Produto Cartesiano dos dois conjuntos.

1. $C$ $\leftarrow$ {&nbsp;} 
2. para cada $x \in$ $A$ faça
3. &nbsp;&nbsp; para cada $y \in B$ faça
4. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;imprima($x$$,y$)
5. &nbsp;&nbsp; fim
6. fim


Explicação:

O algoritmo de Produto Cartesiano realiza o produto cartesiano entre dois conjuntos. O algoritmo recebe como parâmetro dois conjuntos A e B sob os quais o produto cartesiano será realizado. Utilizando um loop controlado o primeiro conjunto (a) recebido como parâmetro na função é percorrido, dentro do loop controlado do primeiro conjunto (a), o segundo conjunto (b) recebido como parâmetro na função também é percorrido, e para cada um dos seus elementos em suas respectivas posições, a função imprima é responsável por criar o par com o elemento da iteração do primeiro (a) com o segundo (b) conjunto. Ao final do algoritmo, tem-se o produto cartesiano do conjunto A sob o conjunto B.

Código em Python
```python
def pCartesiano(A, B):
    for x in A:
        for y in B:
            print('(x:{0} y:{1})'.format(x, y))
```


### Algoritmo 5: Complemento();

// Programa que retorna o complemento entre dois conjuntos.
	sub-rotina complemento (c1, c2 numerico):
		declare c3 numerico
		c3 <- {}
		para e em c1 faca:
			se e nao esta em c2:
				escreva e no final de c3
		retorne c3
	fim_sub_rotina
fim_algoritmo


### Algoritmo 6: ConjuntoDasPartes

### Algoritmo 7: UniãoDisjunta(A, B);
>Entradas: A e B são conjuntos 
Saída: o conjunto resultante da união disjunta entre os conjuntos.

1. $C \leftarrow$ {&nbsp;}
2. para cada $a \in A$ faça
3. &nbsp;&nbsp; Insere()
