# SSC0180-Fonte-Tensao-Ajustavel

## Objetivos
Montar/esquematizar uma fonte de tensão ajustável (corrente continua)  entre 3V a 12V com capacidade de 100mA em 12V

## Componentes
Componente     | Quantidade | Preço Total(R$)
---            | ---        | ---
Transformador 15v 500ma | 1          | 31,60
Diodos 1N4007           | 4          | 0,40
Capacitor 470uF 25v     | 1          | 0,41
Resistor 470ohms        | 1          | 0,05
Diodo Zener 13v 0,5w    | 1          | 0,08
Potenciômetro 1k        | 1          | 1,99
Resistor 390ohms        | 1          | 0,05
Transistor NPN 45v500mA | 1          | 0,20
TOTAL | -- | 34.78

* Transformador.  
O transformador escolhido é o componente responsavel por abaixar a tensão da tomada (220 V) para uma tensão mais proxima da que que será trabalhada (12-3 V). O transformador em questão leva 110 ou 220 para 15V.

[link para compra](https://www.baudaeletronica.com.br/transformador-trafo-500ma-15v.html)
 
* Diodos.  
Os diodos são usados para formar a ponte retificadora/ ponte de diodos. Essa ponte é responsavel por proporcionar o maior aproveitamento da energia, abastecendo o circito com a corrente em ambos os ciclos da corrente alternada. O escolhido para o projeto é o diodo 1N4007.

[link para compra](https://www.baudaeletronica.com.br/diodo-1n4007.html)

* Capacitor.  
O capacitor é responsavel por carregar o sistema quando a tensão (vinda da ponde de diodos) está em declinio estabilizando a tensão que vai para o restante do circuito e criando o "ripple". 
[link para compra](https://www.baudaeletronica.com.br/capacitor-eletrolitico-470uf-25v.html)

.[link para compra]()
.
.

![image](https://github.com/natalzera/SSC0180-Fonte-Tensao-Ajustavel/blob/main/img/circ%20Fonte.png)


[Circuito simulado no falstad](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWcAOaAmA7MgnGB-kA2MAFgwTRBMJCRIGZaBTAWjDACgB3K5SENMmRUwNQcMgd6JEAC8mAOyYAnNvRYyIYaBlL0KyMNkFh4aVhigDY8W3cjJNjTrJFihbgWhmV5S1WDqJBzKnqL8JKJeMhEYkjwIJD4eJHwCHvG0SeCE-ImaxlDcnmjeVKnRRaH5lTXiVmBomZE04VmauUUALlTYYg7tAgP8ECyE0IYYaNgUJJB9eI1QOqTYkIn09KQYGITIlKb8ACZMAGYAhgCuADZdHADGIPoHnc-pEsvwZODYOrmQYHI9EIazQhF2nwBxVKmghTWEgJomRhQ2EKMRRR49CaAimqNxlEy2P48KeOMwhOhePqb3qyLxbTebUkRzJJIGFJyJJAJwuNzurM5aAQYjKpMovKutw4gupIrZ+IlZylAsq4oZnSVfOlADdwNlOaRYUjwCBXqYrPwYAgOAAVfXGxV4iKfPYkQnoLZ8AHIaTYDD0bCbSwsGCQQjg4w7QgikFrEhIGDYZMhXgklJpbxWp5rYpJNFlfPgCH0yjCsTUjIcQEyVIjCF1ypaeCQpAAJSYAGcAJadrrnBT3Jh5ioYxsYyQADwdOTRS0BEBkwltygHndOAHtlABbc5HLcAHU7eAAahxp1mBBb6Osr4wlyAAAobhRdJhHjtdbunbv3Pdb85zyeecKBzA58CoEBhAAYXOAAHc57m7LpD07E4jwAMW7W5VwAcyYbcgMDbAnkgSgGCQG86CgkAAC1FBUI9Ah1ID3SQPBKAQG9wAgh9n1fAArwduw3bcmC6ZQNyYgBrD8mFwm5-2UID8BI7wkAQTMKgfWDlFwwCsVA+oWneTEnlAtoTOZDgNyGM0YioeZhGJZYIG5HFGFtRROwAY6ktDziPFDdyOQDbJI7ErDmbBhDmVzTUoCKQC8hRfP8+CAGfOyPQL12wiTznwwjbJoQgHOitErXQAQapoTzvL8o8FFyv89MAoA)

**Projeto do Esquemático e do PCB no EAGLE**

**Incluir um VIDEO mostrando o Projeto funcionando e/ou simulando, e explicando porque escolheu os valores dos componentes (Upa o vídeo no Youtube ou google drive e poe um link no Readme do teu Github/gitlab).**

## O grupo

André Molina Gregório

Adalton de Sena Almeida Filho

Lucas da Silva Claros

Gabriel Natal Coutinho
