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
Resistor 10ohms         | 1          | 0,05
Transistor NPN 45v500mA | 1          | 0,20
TOTAL | -- | 34.75

..* Transformador
O transformador escolhido é o componente responsavel por abaixar a tensão da tomada (220 V) para uma tensão mais proxima da que que será trabalhada (12-3 V). O transformador em questão leva 110 ou 220 para 15V.

[link para compra](https://www.baudaeletronica.com.br/transformador-trafo-500ma-15v.html)

1. tes
2. te
..* Diodos
Os diodos são usados para formar a ponte retificadora/ ponte de diodos. Essa ponte é responsavel por proporcionar o maior aproveitamento da energia, abastecendo o circito com a corrente em ambos os ciclos da corrente alternada. O escolhido para o projeto é o diodo 1N4007.

[link para compra](https://www.baudaeletronica.com.br/diodo-1n4007.html)

..* Capacitor
O capacitor é responsavel por carregar o sistema quando a tensão (vinda da ponde de diodos) está em declinio estabilizando a tensão que vai para o restante do circuito e criando o "ripple". 

.
.
.

![image](https://user-images.githubusercontent.com/70608303/126587615-77a5b935-c136-45e0-a507-f490d6816679.png)


[Circuito simulado no falstad](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWcAOaAmA7MgnGB-kA2MAFgwTRBMJCRIGZaBTAWjDACgB3K5SENMmRUwNQcMgd6JEAC8mAOyYAnNvRYyIYaBlL0KyMNkFh4aVhigDY8W3cjJNjTrJFihbgWhmV5S1WDqJBzKnqL8JKJeMhEYkjwIJD4eJHwCHvG0SeCE-ImaxlDcnmjeVKnRRaH5lTXiVmBomZE04VmauUUALlTYYg7tAgP8ECyE0PT0kCSQCLmQ9Lr0jUgwuqm4k5hYkISElKb8ACZMAGYAhgCuADZdHADGIPoHnc-pElA205ZG6HtJ2AQyAwqUIjhoMDgnB4pU0GH6wjA8KKMLKTWEsPAyMy9CaAgwlHR+MoOLxRNx-EwJOKVPeTwodMytLabzakiOTzJA2ZnUoJwuNzuHNpaDmlSJfLOV1uHGFBIEYopQwxIH50qF4u58rakoFMoAbuBsszskiIeAQK9TFZ+DAEBwACpGuEI4lWGKwMEkEmwEhAwggmbGEjYPhkaylabUabGBALQKsKIwbApkK8SkpNLeW1UODFJIYsoFrEQmny0VicsZDhImSpEbI+uVLTwT6IEAAJSYAGcAJbdrrnBT3Jj5ipm9MlooAD2dOQxjSxEBkwgdyiH3dOAHtlABbc5HHcAHW7eAAahxZ9mBNapkg0IEqCBhAAFLcKLpME9drq9069+4Dx3c5LyeRc8EoehCjwOhnxAABhc4AAdznuXsumPbsThPAAxXtbnXABzJhd1AqDsCeSBKAYJA7yfYQAC1FBUE9An1UDvSQCDaCmcB8HokA3w-AAr4dey3XcmC6ZQt1YgBrb8mEIm4gOUUD8Ao7wkCBSkKhXBDzmUQiQJ4N56haRlilZToLLZDgtyGS0YlzUNOVtaAIEpRzGAdRRuwAY9krDzhPDD9yOECHIo3F3UgVyZk+LQBBAaKQF8hQAqC5CAGfuxPELN3w6TzmI0iHJoQhnKDDF3MJZKaB8vzApPBQCsAoyQKAA)

**Projeto do Esquemático e do PCB no EAGLE**

**Incluir um VIDEO mostrando o Projeto funcionando e/ou simulando, e explicando porque escolheu os valores dos componentes (Upa o vídeo no Youtube ou google drive e poe um link no Readme do teu Github/gitlab).**

## O grupo

André Molina Gregório

Adalton de Sena Almeida Filho

Lucas da Silva Claros

Gabriel Natal Coutinho
