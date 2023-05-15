# Mini-Curso-de-Animações
Repositório criado para o vídeo mini curso de animações CSS.


---

## Transform

É uma propriedade utilizada para definir modificações aos objetos. Ela pode receber vários atributos, entre eles:

- Translate
- Scale
- Rotate
- Skew

---

### Translate 

Move o objeto em uma quantidade de pixels para uma determinada direção sem mudar o tamanho do box. 
Há três variações desse comando, o `translateX`(move de acordo com o eixo X), o `translateY`(move de acordo com o eixo Y) e o `translate` (que recebe dois valores separados por vírgula, o primeiro é X e o segundo é Y).

---

### Scale

Altera as proporções do objeto. Recebe um valor sem unidade de medida que será utilazo para multiplicar o tamanho do objeto. Também possui as mesmas variações do `translate`.

---

### Rotate

Rotaciona o elemento na medida definida em `deg` (graus) ou `turn` (volta). 

---

### Skew

Inclina um objeto em uma determinada direção.

---

Obs: Além disso, é possível combinar cada um deles, só é necessário tomar cuidado ao sobrescrever o valor de um transform, pois se passarmos apenas um dos valores, os outros serão ignorados. 


---

## Transition

É um conjunto de propriedades que definem como será a transição do objeto:

---

### Transition-property

Permite escolher quais propriedades passarão pela transição. Se quisermos passar mais de uma propriedade, basta acrescentá-la usando vírgula.

---

### Transition-duration

Define a duração da transição. Caso deseje acrescentar tempos diferentes para cada propriedade, basta acrescentar o valor usando vírgula

---

### Transition-delay

Define um delay para o início de uma animação.

---

### transition-timing-function

Define uma função de tempo específica para um objeto. Nela podemos passar vários valores, incluindo alguns padrões do navegador, que são `ease-in` (suaviza o início da transição), `ease-out`(suaviza o fim da transição), `ease-in-out` (suaviza o início e o fim da animação), entre outros. Também é possível utilizar uma função personalizada através da diretiva `cubic-bezier()` que receberá pontos da curva de animação.


---

## Keyframes e Animation

São dois atributos do CSS que juntos são utilizados para a criação de animações.

---

### Keyframes

É uma diretiva utilizada para especificar o que ocorrerá em uma animação. Nela especificamos o que acontecerá em cada momento da animação. Basta colocar a porcentagem que representará o ponto chave, depois, colocar qual propriedade se modificará. Ao invés de usar porcentagens, é possível também usar as palavras chave `from` e `to`, que representam o início e o fim da animação respectivamente. Quando o início tem o valor de default, é possível até mesmo omitir o valor de `from`.

---

### Propriedades Animation

São um conjunto de propriedades que irão definir os detalhes do funcionamento da animação dentro do objeto.

---

#### Animation-name

Define a animação que será atribuída ao objeto.

---

#### Animation-duration

Define o tempo de duração de uma animação. Recebe valores em `segundo` ou em `milissegundo`.

---

#### Animation-timming-function

Define a progressão da animação durante cada ciclo, ou seja, a função de tempo que será aplicada na animação. Recebe os mesmos valores do `transition-timming-function` e também os valores `steps()`, que define em quantos passos a animação ocorrerá e `linear, que define uma animação sem curvas.

---

#### Animation-delay

Define a quantidade de tempo de espera para a animação iniciar. Aceita valores em `segundos` ou `milissegundos`.

---

#### Animation-iteration-count 

Define a quantidade de vezes que uma animação irá se repetir. Recebe um valor numérico ou o valor `infinite`.

---

#### Animation-direction

Define a direção da animação. Recebe os valores `reverse` (realiza o movimento na direção contrária), `alternate` (começa na direção default, e depois alterna entre default e reverse)
e `alternate-reverse`(começa no reverse e fica alternando).

---

#### Animation-fill-mode 

Define os valores que serão aplicados antes e/ou depois da animação. Recebe os seguintes valores: `forwards` (o último estado da animação deve ser mantido), `backwards` (ao final da animação, o objeto será colocado no início da tela) e `both`  (faz a animação iniciar a partir do ponto inicial do objeto e terminar no fim da tela).

---

#### Animation-play-state

Define o estado da animação, se ela está parada ou se está funcionando. Recebe os estados `running` ou `paused`.

---

#### Animation

Shothand utilizada para agrupar todas as propriedades e facilitar a escrita de código CSS. É possível também omitir as propriedades que não serão utilizadas, basta não escrever nada e colocar o valor válido para a próxima propriedade.