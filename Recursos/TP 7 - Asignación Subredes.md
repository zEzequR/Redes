# **_En función del siguiente esquema de conectividad responde las siguientes consignas_**

![Diagrama Esquema Conectividad Original](/Recursos/Diagrama.png)

> NOTA: Los routers tiene identificada cada interfaz de red con la nomenclatura @n donde “n” es el número de puerto. Es decir: si nos tenemos que referir a la interfaz de Router A que se conecta con la Red I nos estaremos refiriendo a la Interfaz 2 y por lo tanto la podemos identificar ese puerto del router con la nomenclatura RA@2 

1. **Calcular el Gateway de las redes A , B, C y D de manera tal que la ip de cada uno de los Gateways sea la ip máxima asignable menos dos (2) de la red a la que pertenece.**

```
    Gateway red A: 170.16.255.252
    Gateway red B: 200.3.124.60
    Gateway red C: 11.11.15.252
    Gateway red D: 129.30.192.124
```

___

2. **El Gateway de la red K (conexión a internet) es la IP mínima Asignable** 

```
    172.17.0.1/16
```

___

3. **Para las redes F-G-H-I-J-L se cuenta con la siguiente trama 192.168.50.128/25, asignar a cada una de ellas una subred la cual debe ser lo más específica posible, comenzando por la primer subred por la red F y asignar las siguiente en orden consecutivo.**

```
    Trama: 192.168.50.128
    Máscara: /25
    Máscara nueva: /30
    Cantidad de subredes: 2⁵ = 32
    Cantidad de IP ́s por subred: 4
    Host asignables: 4 - 2 = 2
```
| Red      | Subred   | Red      | Host 1   | Host 2   | Broadcast|
|----------|----------|----------|----------|----------|----------|
| F |192.168.50.128/30 | .128 | .129 | .130 | .131|
| G | 192.168.50.132/30 |.132 | .133 | .134 |.135|
| H | 192.168.50.136/30 | .136 | .137 | .138 | .139 |
| I | 192.168.50.140/30 | .140 | .141 | .142 | .143 | 
| J | 192.168.50.144/30 | .144 | .145 | .146 | .147 |
| L | 192.168.50.148/30 | .148 | .149 | .150 | .151 |

___

4. **Asignar las direcciones IP a cada boca de los Routers teniendo en cuenta las siguientes opciones:**
<br>
**RA → Boca Red F: IP mínima asignable**
```
    192.168.50.129
```
<br>
**RA → Boca Red I: IP máxima asignable**
```
    192.168.50.142
```
<br>
**RB → Boca Red G: IP máxima asignable**
```
    192.168.50.134
```
<br>
**RB → Boca Red J: IP mínima asignable**
```
    192.168.50.145
```
<br>
**RC → Boca Red H: IP mínima asignable**
```
    192.168.50.137
```
<br>
**RC → Boca Red L: IP mínima asignable**
```
    192.168.50.149
```

___

5. **Asignar a los hosts de las redes A B C y D la IP mínima disponible**

```
Host red A: 170.16.128.1/17
Host red B: 200.3.124.1/26
Host red C: 11.11.0.1/20
Host red D: 129.30.192.65/26
```

___

6. **Armar un nuevo esquema de conectividad con la asignación de IP a cada uno de los dispositivos.**

![Esquema Conectividad Nuevo](/Recursos/esquemaConectividad.svg)

___