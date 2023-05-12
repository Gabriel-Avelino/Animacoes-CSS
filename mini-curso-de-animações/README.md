# Mini-Curso-de-Animações
Repositório criado para o vídeo mini curso de animações CSS.

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