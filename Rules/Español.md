# Reglas

Captura la <span class="color-secundary">bandera</span> de tu oponente con la ayuda de tu <span class="color-secundary">robot</span> para ganar!

## 1. Iniciando una partida

Cada jugador posiciona su <span class="color-secundary">robot</span> en su respectiva <span class="color-secundary">casilla de inicio</span> y su <span class="color-secundary">bandera</span> en la <span class="color-secundary">casilla base</span>. Luego, posiciona su <span class="color-secundary">barricada</span> de manera que su oponente no pueda ver su <span class="color-secundary">buffer</span>.

## 2. Turnos

Al inicio de cada turno, cada jugador posiciona sus <span class="color-secundary">comandos</span> en su <span class="color-secundary">buffer</span>. Hay 6 tipos de <span class="color-secundary">comandos</span> posibles:

* <span class="color-primary">Arriba</span>: Mueve tu <span class="color-secundary">robot</span> una casilla hacia <span class="color-primary">arriba</span>
* <span class="color-primary">Abajo</span>: Mueve tu <span class="color-secundary">robot</span> una casilla hacia <span class="color-primary">abajo</span>
* <span class="color-primary">Izquierda</span>: Mueve tu <span class="color-secundary">robot</span> una casilla hacia la <span class="color-primary">izquierda</span>
* <span class="color-primary">Derecha</span>: Mueve tu <span class="color-secundary">robot</span> una casilla hacia la <span class="color-primary">derecha</span>
* <span class="color-primary">Nada</span>: Tu <span class="color-secundary">robot</span> no realiza ninguna acción
* <span class="color-primary">Disparo</span>: Tu <span class="color-secundary">robot</span> realiza un <span class="color-primary">disparo</span> afectando las casillas en un patrón estilo cruz, igual que el rango de una torre en ajedrez. Esto incluye todas las casillas a su <span class="color-primary">izquierda</span>, <span class="color-primary">derecha</span>, <span class="color-primary">arriba</span> y <span class="color-primary">abajo</span>. Si su oponente recibe un <span class="color-primary">disparo</span> regresará a su casilla inicial

<span class="color-alert">Atención!</span> No te puedes mover hacia una pared, una casilla ocupada por tu oponente estacionado, tu <span class="color-secundary">bandera</span> y hacia una casilla a la que tu oponente también se está moviendo. En caso que esto suceda, tu <span class="color-secundary">robot</span> rebotará hacia su casilla de origen y el juego continuará normalmente.

Cuando ambos estén listos, revelarán sus <span class="color-secundary">comandos</span> al mismo tiempo. Y serán ejecutados uno por uno en el orden de su respectivo <span class="color-secundary">buffer</span>.

<span class="color-alert">Atención!</span> Los <span class="color-secundary">comandos</span> de movimiento tienen prioridad sobre los <span class="color-primary">disparos</span>. Esto significa que cada vez que tu ejecutas un par de <span class="color-secundary">comandos</span> (el tuyo y el de tu oponente) primero ejecutarán los de movimiento (<span class="color-primary">arriba</span>, <span class="color-primary">abajo</span>, <span class="color-primary">izquierda</span>, <span class="color-primary">derecha</span>) y luego los <span class="color-primary">disparos</span> en caso de haber uno.

## 3. Ganar el juego

Primero captura la <span class="color-secundary">bandera</span> de tu oponente posicionando tu <span class="color-secundary">robot</span> en la misma casilla de la <span class="color-secundary">bandera</span>. Una vez capturada, la <span class="color-secundary">bandera</span> se moverá junto a tu <span class="color-secundary">robot</span>. Lleva la <span class="color-secundary">bandera</span> de tu oponente hacia tu <span class="color-secundary">casilla base</span> antes que tu oponente para ganar!

## Qué pasa si...

<span class="color-third">Qué pasa si</span> ambos <span class="color-secundary">robots</span> llevan la <span class="color-secundary">bandera</span> a su <span class="color-secundary">casilla base</span> al mismo tiempo?

<span class="color-third">R/</span> Empate! Juega otra ronda para desempatar!

<span class="color-third">Qué pasa si</span> recibes un <span class="color-primary">disparo</span> mientras cargas la <span class="color-secundary">bandera</span>?

<span class="color-third">R/</span> Tu <span class="color-secundary">robot</span> soltará la <span class="color-secundary">bandera</span>! Esto significa que tu <span class="color-secundary">robot</span> regresará a la <span class="color-secundary">casilla de inicio</span> y la <span class="color-secundary">bandera</span> permanecerá en la casilla donde se recibió el <span class="color-primary">disparo</span>.

<span class="color-third">Qué pasa si</span> recibes un <span class="color-primary">disparo</span> pero aún tienes <span class="color-secundary">comandos</span> pendientes de ejecutar en el <span class="color-secundary">buffer</span>?

<span class="color-third">R/</span> Continúa ejecutándose normalmente! Pero relativamente a la nueva posición de tu <span class="color-secundary">robot</span>.

<span class="color-third">Qué pasa si</span> recibes un <span class="color-primary">disparo</span> y tu casilla inicial está ocupada por tu oponente o tu <span class="color-secundary">bandera</span>?

<span class="color-third">R/</span> En este caso específico tu oponente gana! No puedes estar en la misma casilla que tu oponente o tu <span class="color-secundary">bandera</span> así que ten cuidado!

## Glosario

* <span class="color-secundary">Robot</span>: Personaje jugable. Outbuffered es un juego de 2 jugadores y cada uno controla su <span class="color-secundary">robot</span>. <img src="../PNG/renders/robo.png" height="50"/>
* <span class="color-secundary">Bandera</span>: Cada jugador tiene su <span class="color-secundary">bandera</span>, el objetivo del juego es traer la <span class="color-secundary">bandera</span> de tu oponente a tu <span class="color-secundary">casilla base</span>. <img src="../PNG/renders/flag.png" height="50"/>
* <span class="color-secundary">Casilla base</span>: Casilla donde tu <span class="color-secundary">bandera</span> está posicionada al inicio del juego y donde debes traer la <span class="color-secundary">bandera</span> de tu oponente para ganar.
* <span class="color-secundary">Casilla de inicio</span>: Casilla especial donde los <span class="color-secundary">robots</span> están ubicados al inicio.
* <span class="color-secundary">Comando</span>: Acción que tu <span class="color-secundary">robot</span> ejecutará. Para ejecutar un <span class="color-secundary">comando</span>, posiciónalo boca arriba en tu <span class="color-secundary">buffer</span>. <img src="../PNG/renders/command2.png" height="50"/>
* <span class="color-secundary">Buffer</span>: Porta commandos, cada turno tú eliges los <span class="color-secundary">comandos</span> y los posiciones en tu <span class="color-secundary">buffer</span> en el orden correspondiente de inicio hasta el final. <img src="../PNG/renders/buffer.png" height="50"/>
* <span class="color-secundary">Barricada</span>: Barrera usada para que tu oponente no pueda ver los <span class="color-secundary">comandos</span> mientras los posicionas en tu <span class="color-secundary">buffer</span>. <img src="../PNG/renders/barricade.png" height="50"/>

<style>
.color-primary{
  color: #c1d82fff;
}
.color-secundary{
  color: #aa54d2ff;
}
.color-third{
  color: #00c3c8ff;
}
.color-alert{
  color: #e70029ff;
}
</style>