# SSC0180-Fonte-Tensao-Ajustavel

## Objetivos
Montar/esquematizar uma fonte de tensão ajustável (corrente contínua)  entre 3V a 12V com capacidade de 100mA em 12V

## Componentes
Componente     | Quantidade | Preço Total(R$)
---            | ---        | ---
Transformador 15V 500mA | 1          | 31,60
Diodos 1N4007           | 4          | 0,40
Capacitor 470uF 25V     | 1          | 0,41
Resistor 470ohms        | 1          | 0,05
Diodo Zener 13V 0,5W    | 1          | 0,08
Potenciômetro 1k        | 1          | 1,99
Resistor 390ohms        | 1          | 0,05
Transistor NPN 45v500mA | 1          | 0,20
TOTAL | -- | 34.78

* Transformador.  
O transformador escolhido é o componente responsavel por abaixar a tensão da tomada (220 V) para uma tensão mais proxima da que que será trabalhada (12-3 V). O transformador em questão leva *110V ou 220V para 15V*.  
[link para compra](https://www.baudaeletronica.com.br/transformador-trafo-500ma-15v.html)
 
* Diodos.  
Os diodos são usados para formar a ponte retificadora/ ponte de diodos. Essa ponte é responsavel por proporcionar o maior aproveitamento da energia, abastecendo o circito com a corrente em ambos os ciclos da corrente alternada. O escolhido para o projeto é o *Diodo 1N4007*.  
[link para compra](https://www.baudaeletronica.com.br/diodo-1n4007.html)

* Capacitor.  
O capacitor é responsavel por carregar o sistema quando a tensão (vinda da ponde de diodos) está em declinio, estabilizando a tensão que vai para o restante do circuito e criando o "ripple". O capacitor escolhido é um de 470uF, para criar um riplle de até 10%
[link para compra](https://www.baudaeletronica.com.br/capacitor-eletrolitico-470uf-25v.html)

* Resistores.  
O circuito implementa 2 resistores.  
O primeiro, *de 470ohms*, é responsavel por limitar a corrente passando pelo diodo Zener e pelo potenciômetro. Esse valor foi calculado para causar uma queda de tensão de até 5V quando o ripple esta no minimo (~18V).  
O segundo, *de 390ohms*, limita a tensão minima para aproximadamente 3,7V, fazendo com que o potencial de saida do potenciômetro esteja sempre entre ~12,7 ~3,7V.  
[link para compra (470ohms)](https://www.baudaeletronica.com.br/resistor-470r-5-1-4w.html)  
[link para compra (390ohms)](https://www.baudaeletronica.com.br/resistor-390r-5-1-4w.html)  

* Diodo Zener  
O diodo Zener é usado como limitador de tensão no circuito. O diodo escolhido tem tensão de regulação de 13V, ou seja, ele limita a tensão na saida dele a 13V constantes. Ele sera usado para causar uma tensão de referência para o transistor. O escolhido foi o *Diodo Zener BZX55C*.  
[link para compra](https://www.baudaeletronica.com.br/diodo-zener-bzx55c-13v-0-5w.html)

* Potenciômetro  
O potenciômetro recebe a corrente em paralelo com o diodo Zener, e por tanto tem potencial fixo em aprimadamente 13V (ocorre uma pequena queda do potencial devido as conexões do componente no resto do circuito, mas essa é negligenciavel para nossas aplicações). Assim, ele contrala a tensão mínima (~3V) e máxima (~12V) que vai para o transistor de controle.  
[link para compra](https://www.baudaeletronica.com.br/potenciometro-linear-rotativo-de-1k-1000.html)

* Transistor  
Por fim, o transistor é responsavel por amplificar a corrente que passa pela carga. Utilizando a corrente que passa pela base como referência, ele amplifica essa em 100 vezes. No pior caso (12V) ele recebe 1mA na base, e emite 100mA pelo emissor. O transistor escolhido foi o *Transistor NPN BC337*.  
[link para compra](https://www.baudaeletronica.com.br/transistor-npn-bc337.html)


![image](https://github.com/natalzera/SSC0180-Fonte-Tensao-Ajustavel/blob/main/img/circ%20Fonte.png)


[Circuito simulado no falstad](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWcAOaAmA7MgnGB-kA2MAFgwTRBMJCRIGZaBTAWjDACgB3K5SENMmRUwNQcMgd6JEAC8mAOyYAnNvRYyIYaBlL0KyMNkFh4aVhigDY8W3cjJNjTrJFihbgWhmV5S1WDqJBzKnqL8JKJeMhEYkjwIJD4eJHwCHvG0SeCE-ImaxlDcnmjeVKnRRaH5lTXiVmBomZE04VmauUUALlTYYg7tAgP8ECyE0IYYaNgUJJB9eI1QOqTYkIn09KQYGITIlKb8ACZMAGYAhgCuADZdHADGIPoHnc-pEsvwZODYOrmQYHI9EIazQhF2nwBxVKmghTWEgJomRhQ2EKMRRR49CaAimqNxlEy2P48KeOMwhOhePqb3qyLxbTebUkRzJJIGFJyJJAJwuNzurM5aAQYjKpMovKutw4gupIrZ+IlZylAsq4oZnSVfOlADdwNlOaRYUjwCBXqYrPwYAgOAAVfXGxV4iKfPYkQnoLZ8AHIaTYDD0bCbSwsGCQQjg4w7QgikFrEhIGDYZMhXgklJpbxWp5rYpJNFlfPgCH0yjCsTUjIcQEyVIjCF1ypaeCQpAAJSYAGcAJadrrnBT3Jh5ioYxsYyQADwdOTRS0BEBkwltygHndOAHtlABbc5HLcAHU7eAAahxp1mBBb6Osr4wlyAAAobhRdJhHjtdbunbv3Pdb85zyeecKBzA58CoEBhAAYXOAAHc57m7LpD07E4jwAMW7W5VwAcyYbcgMDbAnkgSgGCQG86CgkAAC1FBUI9Ah1ID3SQPBKAQG9wAgh9n1fAArwduw3bcmC6ZQNyYgBrD8mFwm5-2UID8BI7wkAQTMKgfWDlFwwCsVA+oWneTEnlAtoTOZDgNyGM0YioeZhGJZYIG5HFGFtRROwAY6ktDziPFDdyOQDbJI7ErDmbBhDmVzTUoCKQC8hRfP8+CAGfOyPQL12wiTznwwjbJoQgHOitErXQAQapoTzvL8o8FFyv89MAoA)

------------------------------
### Projeto esquemático
![Projeto esquemático](https://user-images.githubusercontent.com/70608303/126671902-8b6510ad-0f59-4bd4-9217-33f732d51950.png)

------------------------------
### PCB
![Esquema PCB](https://user-images.githubusercontent.com/70608303/126675748-d83f2c4b-78fe-43f4-a76a-9daf7208f5aa.png)


## Calculos dos componentes
<img src="https://user-images.githubusercontent.com/70608303/126670039-9c829897-8d2a-4eb2-a3eb-533e1ae7d988.jpg" aling="left" alt="Cálculo para os resistores" border="0" width="497" height="700">.
<img src="https://user-images.githubusercontent.com/70608303/126669973-f4bc9f7d-e9a4-42b9-914a-477148cf743f.jpg" aling="left" alt="Cálculo para os resistores" border="0" width="497" height="700">.


## Video de explicação do circuito ainda será gravado.

## O grupo

André Molina Gregório

Adalton de Sena Almeida Filho

Lucas da Silva Claros

Gabriel Natal Coutinho
