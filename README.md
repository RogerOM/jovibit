
> Abra esta pagina en [https://ART2BIT.github.io/jovibit/](https://ART2BIT.github.io/jovibit/)

# Art2Bit - JoviBit

## Bloques

### ``moverServo``

```blocks
for (let index = 0; index < 8; index++) {
        JoviBit.moverServo(Pin.P0, 125)
        basic.pause(200)
        JoviBit.pararServo(Pin.P0)
    }
```

El bloque ``moverServo`` tiene un rango de 0 a 180, donde 90 es el punto medio y para la rueda del servo.

### ``NeoPixel``

```blocks
let led: JoviBit.led = null
basic.forever(function () {
    led = JoviBit.create(NeoPixelMode.RGB)
    led.showColor(NeoPixelColors.Blue)
    led.setBrightness(20)
    led.show()
    led.setPixelColor(1, JoviBit.rgb(40, 4, 80))
    led.show()
})
```

Para poder iniciar NeoPixel y dar color al led de la placa de extensión debemos utilizar la funcion ``create``.
Cada vez que se modifique el color o la intensidad, se debe llamar bloque ``show``

## Usar como extensión

Este repositorio puede ser añadido como una **extensión** en MakeCode.

* abra [https://makecode.microbit.org/](https://makecode.microbit.org/)
* haga clic en **New Project**
* haga clic en **Extensiones** en el menú del engranaje
* buscar **https://github.com/ART2BIT/jovibit** e importar

## Edita este proyecto ![Insignia de estado de compilación](https://github.com/ART2BIT/jovibit/workflows/MakeCode/badge.svg)

Para editar este repositorio en MakeCode.

* abra [https://makecode.microbit.org/](https://makecode.microbit.org/)
* haga clic en **Import** luego haga clic en **Import URL**
* pegue **https://github.com/ART2BIT/jovibit** y haga clic en importar

#### Metadatos (utilizados para búsqueda, renderizado)

* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
