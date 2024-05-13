---
title: 'Reparación - Sega Genesis (Golden Axe): Pantalla negra'
visible: true
published: true
taxonomy:
    category:
        - Sega
        - Genesis
    tag:
        - Reparación
    author:
        - Spacemx
routes: {  }
media_order: 'SoldaduraFria.PNG,cart.jpg,genesis_goldenaxe_label.jpg'
date: '24-02-2021 11:13'
---

#### Descripción del problema

##### Pantalla negra

Al conectar el cartucho Golden Axe en la consola Sega Genesis el juego no funciona, es decir que no manda señales de video ni se perciben sonidos, solo muestra una pantalla negra. Esta misma falla se puede presentar en cualquier otro cartucho de juego de Sega Genesis o de cualquier otra compañía. Por lo tanto el diagnóstico y posible solución al problema aplica para otras plataformas basadas en cartuchos.

![Golden Axe](/assets/images/2024-05-08-Golden-Axe/genesis_goldenaxe_label.jpg?resize=400,400)

#### Causas posibles

Usualmente la falla en cartuchos suele presentarse a causa de:
1. Suciedad (óxido/corrosión) en los conectores
2. Soldadura fría o deficiente en algún componente interno.
3. Pistas de conexión dañadas, algunas causas pueden ser rasguños, daño físico por golpes, corrosión, óxido, líquidos derramados en su interior, etc..
4. Algún componente interno dañado, que pueden ser:
* ROMs (mask ROM con los datos del juego)
* Circuitos integrados como el 74LS00
* resistencias
* capacitores
* circuitos de reloj (cristal oscilador)
* Circuitos personalizados (custom) de seguridad o especial para procesamiento de gráficos.
5. Otro factor de falla es tener una ROM con datos incorrectos o dañados.

#### Diagnóstico y reparación

Al abrir el juego notamos que aparentemente todo estaba bien, pero al revisar con mas detalle pudimos notar soldadura fría en algunos pines que conectan a la MASKROM con la tarjeta, es decir que ha perdido su brillo y flexibilidad por lo cual se nota opaca y agrietada, revelando claramente un falso contacto ocasionando falta de conductividad.

![Soldadura fría](/assets/images/2024-05-08-Golden-Axe/SoldaduraFria.PNG)

Motivo por el cual se recomienda hacer renovación de soldadura de todos los pines de la ROM en la pcb y no solamente en los detectados con falla. Esto debido a que si se tienen un par de pines con soldadura fría, es muy probable que en el futuro otros pines lleguen a presentar esta condicion al haber sido soldados en la misma fecha en toda la placa.

Si el problema es muy severo, es decir cuando la soldadura está muy sucia o reseca y al aplicar calor se vuelve arenosa, lo ideal es remover por completo la soldadura vieja para posteriormente aplicar nueva (aleación estaño/plomo) en cada conector y con esto cumplir a cabalidad con el término de renovación de soldadura.

Aunque en la mayoría de los casos puede ser suficiente agregar flux a los conectores con falla y fundir la misma soldadura que tiene el pin en cuestión y se corrige la continuidad. 

Posteriormente hacemos limpieza para eliminar residuos de soldadura y flux y verificamos conductividad en todos  los pines y circuitos internos para descartar que la falla se presente por este concepto.

Ensamblamos el cartucho y hacemos la prueba final. En nuestro caso podemos confirmar que ahora funciona correctamente el juego Golden Axe de Sega Genesis.

###### @Spacemx
