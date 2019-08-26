# Estudio analógicos:

Nota: todo este documento es un resumen del apunte del curso que a su ez se basa en el Allison.

# Primera parte del curso:


## Radiación de cuerpo negro (pg 1 Allison)


+ Problema: Mecánica clásica falla al predecir energia de radiación de calor

para encontrar la densidad de energía $u(\omega)$ radiada a una frecuencia angular $\omega$

La fórmula de Rayleigh-Jeans es

$$ u (\omega) = \frac{\omega^2Vk_BT}{\pi^2 c^3}$$


Así la energía total emitida por la caja sería derivada de la integral de todas as densidades

$$U= \frac{Vk_BT}{\pi^2c^3}\int_0^\infty \omega^2 d\omega=\infty$$

claramente este resultado no tiene sentido


Esto se arregla tomando la energía en paquetes. Si se supone que la energía de un fotón es: $E=nhf$, donde $f$ es la frecuencia, $h$ es una cte y $n$ es el _número cuántico_ $\in \mathbb{N}^*$

Así para calcular la energía, hay que usar sumatorias en vez de integrales:

$$E_\omega=\frac{\sum_{n=0}^\infty nhfe^{-\frac{nhf}{k_BT}}}{\sum_{n=0}^\infty e^{-\frac{nhf}{k_BT}}}=-hf\frac{d}{d\mu'}\left[ log \sum _ {n=0}^\infty e^{-n\mu'}\right]_{\mu=\frac{hf}{k_BT}}$$

Esta es la distribución de Plank

$$u(\omega)=\frac{\omega^2 V}{\pi ^2c^3}\left(\frac{hf}{e^{hf/k_BT}-1}\right)$$


con $h=6.626 \cdot 10^{-34}[Js]$


## Efecto fotoeléctrico:

Se emite luz a placa de metal, esta emite electrones: li interesante &rarr; es que la energía de los electrones no depende de la intensidad, sino de la frecuencia de la luz, además los electrones son irradiados de manera instantánea. Esto presenta dos contradicciones con la teoría clásica:

1. En la teoría clásica, la energía debería ser proporcional a la intensidad de la onda electromagnética incidente.
2. En teoría clásica, habría un retardo en la emisión de los electrones.

Plank propuso un oscilador que solo puede tener energías $E_n=n \hbar \omega; n\in \mathbb{N}^*$.

Einstein postuló (ganó Nobel por esto): __Una onda electromagnética de frecuencia $\omega$ y energía $n \hbar \omega$ colapsa en (está compuesta de ) $n$ partículas (llamadas fotones) con energía $\hbar \omega$.__ De esto se desprende inmediatamente la cantidad de electrones emitidos y su relación con la intensidad (no con la energía)

Si hay un potencial generado por el metal, que se encarga de quitarle energía al electron que quiere salir, mientras que la luz le otorga energía, así la energía del electron está dada por:

$$E_e=\hbar \omega - \phi$$


## Átomo de Bohr (pg 7 Allison)

Intenta explicar las líneas espectrales de los elementos

si consideramos la atracción de un núcleo de H a su electron que le orbita tenemos que la fuerza entre ambos está dada por Coulomb:

$$\vec{F}=-\frac{q^2}{4\pi \epsilon_0 r^2}=\frac{m_ev^2}{r}$$


 La energía del electron es la suma de la pontencial y kinética:

 $$U=-\frac{q^2 }{4\pi \epsilon_0 r}$$

 $$K=\frac{1}{2}m_ev^2=\frac{q^2}{8\pi \epsilon r}$$

 $$E=-\frac{q^2}{8\pi\epsilon r}$$


Y su frecuencia de rotacion vivne dada por:

$$f=-\frac{v}{2\pi r}=-\frac{q}{4\sqrt{\pi^3 \epsilon_0 m_er^2}}$$


Pero si esto fuese así, el electrón, en clásica, perdería energía en forma de campo magnético y colapsaría, no pudiendo existir.

Si por el contrario, la energía esta en quantos, ahora funciona. La energía para pasar de un nivel a otro viene dada por:

$$E_1-E_2=hf_{12}$$

Asumiendo que el momento angular está cuantizado, tenemos:

$$L=m_evr=n\hbar$$
$$v^2=\frac{n^2 \hbar}{m^2_er^2}$$

## La hipótesis de Louis de Broglie (pg. 12 Allison)

Vimos que la luz se puede comportar como onda o como partícula, y experimentalmente se pueden mover objetos con luz.


### La hipótesis

En palabras simples, la hipótesis de Allison dice lo siguiente:

> "Si fotones de luz con longitud de onda $\lambda$ tienen momentum $p=h/\lambda$, entonces de más que es posible que partículas con momentum $p$ tengan asociada una frecuencia $\lambda$ y se comporten como ondas en ciertas condiciones."
>
> -El xoro de Broglie

Primero tenemos el postulado de Einstein:
$$E=\omega \hbar$$

$$E=pc$$
como la energía en un nivel estable es sólo kinética, ya que no hay pérdida, $p$ es el moméntum y $c$ la vel de la luz.

Luego:

$$p=\frac{\hbar\omega}{c}=\hbar k=\frac{hf}{c}=\frac{h}{\lambda}$$

Pero en principio, $p$ puede serl el momentum de cualquier cosa, como consecuencia de esto, las longitudes de ondas asociadas a objetos cotidianas, son tan pequeñas que es muy dificil de medir y en la mayoría de las circunstancias imposible, peeeero, esto sirve para mostrar que los electrones y fotones no están solos, sino que ¡todas las particulas tienen asociadas longitudes de ondas!

Recordar: $\omega=2\pi f$ y $\hbar=h/2\pi$ &rarr; $E=\hbar \omega$

> Nota: (Todas las fórmulas para el C1 se pueden encontrar en este [formulario](https://github.com/tomasrojasc/apuntes-circuitos-analogicos/blob/master/res%C3%BAmenes/C1/Formulario_C1_por_Camilo_R.pdf).)


Esta hipótesis se pudo comprobar en un experimento donde se dispara luz a un cristal, hay interferencia constructiva si:

$$2d \cos \theta = n \lambda$$

donde $\theta$ es el ángulo de incidencia y $d$ la distancia entre planos cristalinos. Esto si no me equivoco, es lo que se conoce como area transversal de scattering. Dato: Este hecho se usa en cristalografía por difracción de Rayos X, método por el cuál Rosalind Franklin descubrió la estructura molecular helicoidal del ADN en forma B.

De este principio se desprende naturalmente la dualidad Onda Partícula

## Paquetes de onda: velocidades de fase y grupo de las partículas (pg. 16 Allison)

<iframe src="https://www.desmos.com/calculator/9nzn3d3pzp?embed" width="500px" height="500px" style="border: 1px solid #ccc" frameborder=0></iframe>

En el gráfico que se muestra, vemos 7 señales, las primeras 4 son funciones seno con frecuancias muy similares. Las 3 de abajo son: En morado: la suma de las dos primeras señales, en negro la suma de las primeras 3, en rojo la suma de las primeras 4. Vemos que a medida que añadimos ondas que varían poco en la frecuencia, los paquetes de onda van creciendo en aplitua y separándose entre sí. Esto da una intuición que si sumamos infinitas, vamos a quedar con un único paquete de onda.

En teoría cuántica, los paquetes de onda representan objetos con propiedades duales onda partícula.

### ¿Cuál es la velocidad de un paquete de onda?

Tomemos una onda que viaja en sentido positivo en el eje $x$ con la siguiente expresión:

$$A_0 \cos(\omega t -\beta x)$$

$\beta$ es la constante de fase, se relaciona con la longitud de onda de la siguiente manera: $\beta=2\pi/\lambda$. Por lo general es conveniente usar representación exponencial:

$$A_0 Re[\exp(j(\omega t -\beta x)]$$
Donde $j=i$ es la unidad imaginaria (sé que es común, pero aun no me acostumbro). Vamos a omitir la función de la parte real pq es un abuso de notación y un desperdicio de tinta y tecleo.

La propagasión de una onda está determinada por 2 velocidades, las famosas velocidades de grupo y de fase, $v_g$ y $v_f$ respectivamente.

[//]: # (TODO: Acá lo ideal sería motrar un gráfico animado que muestre la diferencia entre la velocidad de fase y la de grupo, ojala replicar lo del video pero en desmos)

<iframe width="560" height="315" src="https://www.youtube.com/embed/tlM9vq-bepA?start=20" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

En este video podemos ver la diferencia entre las dos velocidades antes dichas, podemos ver que pese a que en muchos casos la velocidad de fase es mayor que la de la luz, no implica una transferencia de información más rápida que $c$, por lo que no hay problema acá.

La velocidad de fase se defineniendo en cuenta esto, tenemos que la velocidad de una fase es cuando:

[//]: # (TODO: Explicar bien esto)

$$\omega t - \beta x = \text{constante}$$

Derivando con respecto al tiempo t despejando $dx/dt$ nos queda:

$$v_f=\omega/\beta$$

Notar que la fase acá hace referencia a la frecuencia en el tiempo de una onda. Recordemos $\omega$ es la frecuencia en el tiempo y $\beta$ en el espacio.

[//]: # (TODO: llenar con la pg 19 del allison)

Por otro lado la vel de grupo está dada por:

$$v_g=\partial \omega/\partial\beta$$

Es la velocidad a la que se mueve la energía, y por ende es siempre menor o igual a $c$


Por hipótesis de De Broglie, tenemos que el momentum y la energía de una partícula son:

$$p=mv=h/\lambda$$
$$T=\frac{1}{2}mv^2=hf$$

respectivamente.

Pero también sabemos que una onda plana infinita, está descrita por $A_0\exp[-j(\omega t - \beta x)]$

Como:

$$\beta=\frac{2\pi}{\lambda}=\frac{2 \pi p}{h}=\frac{p}{\hbar}$$

Se intuye la siguiente ecuación:

$$\psi = A_0\exp[-j(Tt-px)/\hbar]$$

Las velocidades asociadas a esta eq de Onda son:

$$v_f= \frac{\omega}{\beta}=\frac{T}{p}=\frac{1}{2}\frac{mv^2}{mv}=\frac{v}{2}$$


En el caso de una partícula individual tenemos que:


$\partial \omega = (mv/\hbar)\partial v$

$\partial \beta =(m/\hbar)\partial v$


Usando esto, tenemos que la velocidad de grupoes:

$$v_g=\partial \omega/ \partial \beta =v$$


## La ecuación de onda de Schrödinger (pg. 21 Allison)

Vimos que las partículas pueden poseer (o derechamente poseen) propiedades duales y que la función de densidad de probabilidad está descrita por una función $\psi$. Esta ecuación incluye la energía kinética de la partícula pero también es posible que haya un potencial asociado. De manera general, la energía de una partícula viene dada por:

$$E=\hbar \omega = T+U$$

Así la función de onda unidimensional, en el caso más general, pasa a ser:

$$\psi = A_0 \exp[-j(Et-px)/\hbar]$$

Si nos preguntamos, a cuál EDP satisface esta ecuación, nos acercamos a la ec del loco del gato.


La ecuación, después de diferenciar una vez c/r a $t$ y dos c/r a $x$ y ver qué faltaba, es:

$$\frac{\partial ^2 \psi}{\partial x^2}-\frac{2m}{\hbar^2}U\psi+j\frac{2m}{\hbar}\frac{\partial \psi}{\partial t}=0$$


En 3D:

$$\nabla^2\psi-\frac{2m}{\hbar^2}U\psi+j\frac{2m}{\hbar}\frac{\partial \psi}{\partial t}=0$$


y en lo personal creo que queda más boni así:


$$\left(\nabla^2+j\frac{2m}{\hbar}\frac{\partial }{\partial t}-\frac{2m}{\hbar^2}U\right)\psi=0$$


Podemos intentar hacer una separación de variables.

$$\psi = \Psi(x)\Gamma(t)$$

Así:

$$\frac{\hbar}{2m}\frac{1}{\Psi}\frac{d^2 \Psi}{dx^2}-V=-j\frac{\hbar}{\Gamma}\frac{d\Gamma}{dt}$$


Así, resolviendo esto, con un potencial $V=V(x)$ podemos igualar cada parte a una cte $C$, así con esto en mente:

$$\Gamma (t)=\exp{(jCt/\hbar)}$$

Comparando con la ec anterior, tenemos $C=-E$

De esta manera:

$$\psi=\Psi(x) \exp{(-jEt/\hbar)}$$


Una vez resuelto $\psi$ tenemos que el cuadrado de la función es la densidad de probabilidad de encontrar una partícula, y la normalizamos para que tenga sentido probabilístico:

$$\iiint_{\Omega}\psi \psi^* dV=1$$
$\Omega \in R^n$

Donde $n=\dim(\text{Espacio})$



## Principio de incertidumbre

Existen pares de variables que no pueden ser medidas experimentalmente con presición arbitraria a la vez:

  1. Por un lado, tenemos el par $(E,t)$
  2. Tenemos el par $(p,x)$

Esta __no__ es una limitación experimental, sino una limitación escencial de la naturaleza.

> Nemotecnia no tan nemotcnia pq tiene sentido físico:
> si vemos la función $\psi=A_0\exp{[-j(Et-px)/\hbar]}$
> Nótese que las cantidades que no se pueden medir con exactitud arbitrariaa la vez están juntas en $\psi$.

Tenemos las siguientes ecuaciones:

$$\Delta E \Delta t \geq h$$

Por otro lado,como ya habíamos visto:

$$\Delta E=h\Delta f=mv \Delta v=v\Delta p$$

$$\Delta p \Delta x \geq \hbar/2$$
