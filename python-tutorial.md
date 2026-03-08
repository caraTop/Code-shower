# **Python Tutorial**

# Setting up
Primeiras coisas primeiro meus fellas,
como colocar o python rodando na sua maquina?
Eu sei que vocês betinhas usam windowns, aqui o [link da pagina da microsoft store](https://apps.microsoft.com/detail/9ncvdn91xzqp):
Isso é python 3.12, "Ah, mas a versão mais recente", não, aqui é 3.12

Baixou? agora rodar essa bagaça
Abre o cdm (Prompt de comand) e escreve "python"
![[Pasted image 20260306215645.png]]
(iguinorem que eu to usando linux gente, o python é igual)
Booom python ja ta rodando
O que for escrito ai, vai rodar, mas é paia né?

Ai que vem o [visual studio code!](https://apps.microsoft.com/detail/xp9khm4bk9fz7q) Escrever nunca foi tão estiloso
Boom, visual
![[Pasted image 20260306220042.png]]
(o de vocês ai vai ter um simbulo diferente por que linux né)
Isso é tipo um gerenciador de arquivo, mais um bloco de notas, mais um corretor de erros
Serve pra deixar sua vida mais facil

Então agora, cria uma pasta no seu computador, e abre ela no vs code
![[Pasted image 20260306220238.png]]
Depois de abrir a pasta vazia, bom ela vai continuar vazia
Cria um arquivo ai
![[Pasted image 20260306220356.png]]
(O primeiro botãozinho ai)
Pode por qualquer nome, só tem que por o .py no final.
(é a extenção do arquivo, tipo txt é de texto, py é python)
![[Pasted image 20260306221446.png]]
Boom, ja ta pronto pra uso, 
no meio te a area de escrever seu codigo,
na esquerda todos seus arquivos,
e na direita o botão de rodar o codigo.

# Extenções no vs
Extenções não são necessarias, elas só servem pra facilitar a vida
![[Pasted image 20260307091619.png]]
Abre as extenções com esse quadradinho aqui, e ai procura o nome
![[Pasted image 20260307091653.png]]
Esta por exemple, serve para auto-completar palavras no codigo
é a unica que vou estar usando mas se sinta livre para baixar o que quiser

# Variaveis & Data types
Todos devem saber o que é uma variavel né? Assumir um nome a um valor para chamalo de novo, simple assim.
Para definir uma variavel é simples, o nome, simbulo de = e o valor
```
Variavel = 1
```
Isso é uma variavel, mas o importante é o que esta dentro dela
O tipo de dado salvo,
Existem os seguintes tipos primarios

## Boolean
Esse é o tipo mais simples, ela pode ser verdadeira ou falsa
True é uma boolean
False é uma boolean
(lembre-se de por a primeira letra maiuscula, se não ela vai ser considerado o nome de uma variavel)
```
bolo = True
torta = False
```
Esta será melhor usada quando entrarmos em logica, então espera ai

## float & int
Esse tipo é para numeros
Float são numeros racionais
Int são numeros inteiros
Por exemplo
1 é int
1.5 é float
1.0 tambem é float
Não precissa colocar nada alem do numero para definir um int ou um float, eles são definidos automaticamente, caso coloque um . ou não
(Vale lembrar que . é a virgula, então 1,5 seria escrito 1.5)
```
x = 1
y = 1.5
z = 1.0
```

## Strings
String são as variaveis de texto
Sendo definidas por aspas simples (') ou dupla ("), elas sobrecedem as os outos tipos
1 é um int
1.5 é um float
True é uma boolean
"1" é uma string
'1.5' é uma string tambem
"True" é uma sting denovo!
Ela é obrigatoria para outros caracteres tambem
palavra é uma variavel
"palavra" é uma string
```
palavra = "palavra"
nome = 'João'
```

## Definir variaveis com variaveis
Se pode dar o valor de uma variavel a outra dessa forma
```
X = 2
y = x
z = "X"
```
Neste caso, 
x e y tem o valor de 2 (int)
e z tem valor de "x" (string)

## Normas de nomenclatura
>"Todas as nomenclaturas são iguais, mas algumas são mais iguais que outras"
-PINHEIRO, Arthur

Eu sei, eu sei, eu sou um genio por pensar em uma citação tao incrivel, não precissam me dizer isso.
Basicamente, você pode dar o nome que quiser pra sua variavel, mas as pessoas podem ficar confusas (ou pode so ficar feio mesmo).
Por isso foi feito uma "norma", ela não é obrigatoria, mas se recomenda caso va mostrar seu codigo para alguem.

- nomes desritivos, tem que ser obivio pra que serve, mas não precissa ser muito grande
- não reutilize a mesma variavel para varias funções, você é um ser civilizado
- evita siglas que só você entende, e de preferencia nomes pronunciaveis
- sem acentos ou outros caracteres especiais

Agora para variaveis que precissam de mais de uma palavra para ser descritiva o suficiente, existem alguns casos, os mais comuns sendo:
- Camel Case: todasAsPalavrasComLetraMausculaExetoAPrimeira
- Pascal Case: TodasAsPalavrasComLetraMauscula
- Snake Case: separadas_por_travesao_e_tudo_minusculo

Eu uso Camel case, e é o que vocês veram nesse turorial,
você pode usar outro (mas sera criticado).

E isso foram variaveis.

# Print & Input
O basico de python, mostrar algo pro usuario, e receber dado do usuario.
Primeiro, vamos rodar o codigo que todos conhecem, Hello word.
Só copiar esta linha aqui e colocar no Vs, (ou terminal se for oq que você escolheu usar)
```
print("Hello World!")
```
Quando você rodar esse codigo no Vs, um terminal vai aparecer em baixo, e o nosso texto estara exibido.
![[Pasted image 20260307093531.png]]
(A linha de cima, é apenas o codigo iniciando, mostrando o lugar do arquivo, independente de que codigo rodar, ele ira aparecer)
Lembrese que deve ser usado ", se não ele vai tentar encontrar uma variavel com este nome.
`NameError: name 'helloWorld' is not defined`
Extato, você pode usar print em variaveis:
```
texto = 'Hello world!'
print(texto)
```
Esse codigo tambem escrevera Hello world! no terminal.
Tambem se pode printar mais de uma variavel de uma vez:
```
textoUm = 'World!'
textoDois = 'Hello'
print(textoDois, textoUm)
```
Basta colocar uma , entre as variaveis .
Isso tambem funicona com a string pura:
```
print("Hello", "World", '!')
```
Agora o input:
Quando input for chamado, um espaço no terminal será colocado para o usuario.
**IMPORTANTE:** O que o usuario escrever será recebido como uma String.
```
input()
```
![[Pasted image 20260307105700.png]]
Esta caixa branca representa que o usuario pode escrever.
O que for escrito dento do parenteses de input() será exibido antes da área de escrita.
```
input('Seu texto aqui: ')
```
![[Pasted image 20260307105840.png]]
Mas por enquanto este valor não esta sendo salvo!
Vamos salvar o valor do input numa variavel, e printar depois para ver se esta sendo salvo mesmo:
```
userInput = input('Seu texto aqui: ')
print(userInput)
```
![[Pasted image 20260307110021.png]]
Pronto, já esta funcionando, e salvando o que foi colocado.

# Modificadores de valores
## Aritmética
Eu sei que todos aqui amam matematica (Sim, todos!), então essa parte deve ser fácil,
Lembrando que isso pode ser feito apenas em numeros, int ou float, e não strings.

Aqui estão os operadores basicos:
| Operação | Operador | exemplo | Função |
| --- | --- | --- | --- |
| Soma | + | 5 + 2 = 7 | Soma dois numeors |
| Subitração | - | 5 - 2 = 3 | Subitrai dois numeors |
| Multiplicação  | * | 5 * 2 = 10 | Multiplica dois numeors |
| Divisão | / | 5 / 2 = 2.5 | Divide dois numeors, (sempre resulta em Float) |
| Floor division | // | 5 // 2 = 2 | Divide dois numeors, iguinora os decimais |
| Module | % | 5 % 2 = 1  | Resulta na sobra de uma divisão |
| Exponente | ** | 5 ** 2 = 25 | Eleva um numero a outro |

(Se você não entendeu algum direito, testa com eles ai, coloca as equações dentro de um print e roda o codigo).
Existem mais operadores, mas esses são os basicos, os mais complexos vamos deixar para depois.

## Modificadores de string
Estes modulos são colocados apos uma string para mexer no que esta escrito dentro:
| Operador | exemplo | Função |
| --- | --- | --- |
|.upper() | texto -> TEXTO | Deixa as letras maiusculas |
|.lower() | TEXTO -> texto | Deixa as letras minusculas |
|.capitalize()| tEXto -> Texto| Deixa a primeira letra maiuscula e o resto minusculo |
|.strip|    texto      -> texto | limpa a string, tira caracteres na frente e atras |

Alguns simbulos aritméticos tambem podem ser usados em string:
O + concatetuna duas strings em uma só.
O * multiplica o numero de vezes que a string é repitida. 


## Conversão
Digamos que eu quero duplicar um numero dado pelo usuario:
```
userInput = input("Escreva um numero: ")
print(userInput * 2)
```
Bom, se você tentar rodar isso, ele vai escrever o numero duas vezes, Afinal como eu disse, inputs resultão em strings, e as equações são numeros, logo, você deve converter:

| Comando | Função |
| --- | --- |
| str() | converte o que esta escrito dento em uma string |
| int() | converte o que esta escrito dento em um inteiro |
| float() | converte o que esta escrito dento em um decimal| 
| bool() | converte o que esta escrito dento em uma Boolean, (Só é False quando é 0 ou uma string vazia "" ou '') |

Então com isso podemos:
```
userInput = input("Escreva um numero: ")
userInput = float(userInput)
print(userInput * 2)
```
E agora o codigo funiona como esperado:
![[Pasted image 20260307113501.png]]
Ou será que não? ([Musica do Vsauce](https://www.youtube.com/watch?v=LB0--7xweG8) começa a tocar) (Sim, valeu a pena pegar esse link do youtube so pra fazer essa piada).
Caso você tente escrever algo que não é um numero:
![[Pasted image 20260307113759.png]]
Um erro, ele tenta converter e não da. Como resolver? Espera e descubra (Fazendo suspense igual novel da globo)

# if & else
