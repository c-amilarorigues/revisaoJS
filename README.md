# Revisão JavaScript

## Números e Strings
 
 JavaScript pode compreender diferentes tipos de dados, como números e strings.
Tente inserir um número no console:
```
> 2
```
Da mesma forma, tente inserir qualquer string no console:

```
> "0lá, mundo."
``` 
Lembre-se, as strings são colocadas entre aspas

## Variáveis

Você pode armazenar dados dentro de contêineres (variáveis) usando "var"

Você pode armazenar seu nome dentro de uma variável?
```
> var name = "Ravi"
```
Agora chame a variável para ver o que há dentro dela.
```
> name
```
Você pode ver seu nome impresso no console.

Strings são objetos em JavaScript e têm algumas propriedades e funções definidas. Você pode experimentar alguns deles.

```
name.length
```
```
name.toUpperCase()
```
Você poderá ver seu nome em letras maiúsculas.

Você também pode armazenar qualquer número dentro da variável.

```
> var num = 5
```

Você também pode converter uma string em um número:

```
parseInt("123")
```

## Operações aritméticas
Você pode usar operações aritméticas em números usando operadores aritméticos (+, -, /, *,%).

_Observação: lembre aos alunos que o sinal do módulo (%) dá a você um resto entre dois números._

Você pode tentar fazer diferentes operações aritméticas no console.  
```
2+3
```
```
2-3
```
```
5*7
```
```
36/12
```
```
12%5
```
Tente usar o operador aritmético '+' em strings e adivinhe o que acontecerá:

```
"Olá" + "Amigo"
```
Strings são unidas quando você as adiciona.

Agora tente usar qualquer outra operação aritmética em strings como divisão (/)

```
"a" / "b"
```
Você obterá **NaN** que significa não um número.

Agora tente dividir qualquer número por 0:

```
1/0
```
Você receberá **Infinity** como uma resposta.

## Booleanos
Há outro tipo de dados booleano em JavaScript que pode conter apenas **true** ou **false**
```
var bool = true
```

Os operadores de comparação (>, <,> =, <=, ===,! =) também avaliam como um valor booleano.
Tente usar qualquer um dos operadores de comparação com números no console
```
2===3
```
Isso imprimirá falso no console.

## Outros tipos de dados
Existem dois outros tipos de dados em JavaScript - **null** e **undefined**

**null** é usado quando você deseja que uma variável não contenha nada.
**undefined** é o valor dentro de uma variável quando você se esqueceu de atribuir algo a ela.

```
var teste
```
Agora tente ver o que está dentro de 'teste'
```
teste
```
## Programação condicional
Podemos usar o bloco if-else para criar programação condicional.
Tente escrever uma declaração if-else simples:
```
if(3>2){
	console.log("Feliz")
}
else{
	console.log("Não Feliz")
}
```
Se a condição for avaliada como **true**, se o bloco for executado; caso contrário, o bloco é executado.

A instrução switch é outra maneira pela qual podemos fazer programação condicional.

```
var name = "Meu nome";

switch(name) {  
case  "Meu nome":  
console.log("Condição 1");  
break;  
case  "meu Nome":  
console.log("Condição 2");  
break;  
default:  
console.log("Nenhuma das condições é verdadeira");
}
```

## Loops
Os computadores não gostam de se repetir. Usamos loops para realizar funções repetidas. Existem dois tipos de loops - loop **for** e **while**.

Escreva um loop **for** simples:

```
for(var i=0; i<=5; ++){
	console.log(i)
}
```

Escreva um loop **while** simples:

```
var i =0
while (i<=5){
	console.log(i)
	i=i+1
}
```

## Matrizes
Matrizes são um tipo de estrutura de dados onde você pode usar uma única variável para armazenar uma lista de itens.

Escreva uma matriz que armazene uma lista de itens.

```
var friends = ["friend1", "friend2", "friend3"]
```
Você pode acessar qualquer item da lista usando índices.
_Observação: A contagem começa em 0 nos computadores_
```
friends[0]
```

Você também pode fazer um loop sobre todos os itens usando o loop **for-each**

```
for(var index in friends){
	console.log(friends[index])
}
```

Matrizes também são objetos em javaScript. Eles têm algumas propriedades e funções definidas.
Por exemplo, você pode obter o comprimento da matriz usando a propriedade length:

```
friends.length
```

Você também pode inserir novos elementos na matriz usando push():

```
friends.push("friend4")
```
Você pode ver os elementos na matriz friends agora:
```
friends
```

Você também pode retirar o último elemento da matriz usando pop():

```
friends.pop();
```

## Funções
Javascript tem certas funções embutidas que você pode usar.
Você também pode escrever suas próprias funções.
Escreva uma função para calcular a circunferência de um círculo. Deve ter raio como argumento.


```
function circumference(radius){
	var circumference = 2 * 3.14 * radius
	return circumference
}
```
Agora você pode usar as funções de circunferência para calcular o raio de qualquer círculo.

```
circumference(5)
```

## Objetos
Usamos classes para projetar projetos de objetos em javascript e, em seguida, usamos **new** para criar um novo objeto usando a classe.

JavaScript cria internamente um novo objeto usando *new Object()*
```
var paddle = new Object();
```
Você pode atribuir novas propriedades e funções ao objeto de teste.

Peça ao aluno para atribuir uma nova propriedade e função a um objeto de teste

```
paddle.length = 60
```

```
paddle.showLength = function(){
	console.log(paddle.length);
}
```

Chame paddle.showLength() para ver o tamanho da raquete.

```
paddle.showLength()
```

Chame paddle object para ver o que está armazenado dentro de paddle (raquete).

```
paddle
```
