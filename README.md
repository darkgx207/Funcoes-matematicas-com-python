# Bem vindo(a) ao tópico de recursividade com Python através de noções de funções matemáticas. 


<img src=https://cdn.pixabay.com/photo/2019/04/14/10/27/book-4126483_960_720.jpg >


## Assim como na matemática, onde representamos as funções da forma $f(x)$ . Podemos pensar nas funções recursivas da mesma forma.

## Imagine a seguinte função:
$$ \text{Dado } x \in \mathbb{Z} \text{ temos que: }
\\ f(x)=f(x-2)+f(x-1) \\ \text{onde, }  f(1)=f(2)=1 \\
$$

### O resultado dessa função são os numeros da sequencia de Fibonacci.
<br/>

## Agora a pergunta é, como escrever código em python *(ou qualquer outra linguagem que aceite recursividade)* da mesma forma que escreveríamos em linguagem matemática?

## Aqui, ao imaginarmos que a sentença a seguir é entendida da seguinte forma:
$$ f(x) = 2x+1 $$ 
```python
def f(x):
    return 2*x + 1
```
### Podemos relacionar a igualdade através do retorno da função.

<br/>

### Dessa forma podemos escrever que

$$ \text{Seja x} \in \mathbb{Z} , \text{ e } f(1)=f(2)=1 $$

$$ f(x) = f(x-2) + f(x-1) $$



```python
def f(x):
    if x== 1 or x==2:
        return 1      # ou seja, f(1)=f(2)=1
    else:
        return f(x-2) + f(x-1)
```
### Como resultado a função irá retornar o x-ésimo valor da sequencia de Fibonacci.
