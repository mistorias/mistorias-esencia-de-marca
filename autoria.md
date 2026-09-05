# Autoría

Cada historia de Mistorias la firma una persona, y esa firma lleva a una ficha
donde quien lee puede saber quién es. Este documento fija qué se le pide a esa
persona, qué no se le pide nunca, y qué se le promete.

Es el criterio editorial. El formato técnico —nombres de campo, dónde va el
archivo— vive en `CLAUDE.md` de
[mistorias-contenido](https://github.com/mistorias/mistorias-contenido), y el
porqué de la decisión técnica en el
[ADR 0016](https://github.com/mistorias/mistorias-web/blob/main/docs/adr/0016-autoria-verificable-de-las-historias.md)
de mistorias-web.

## 1. Por qué firma una persona y no «Mistorias»

La guía editorial pone la **confianza** entre los criterios de marca: fuentes
visibles, contexto explicado, honestidad sobre los límites de los datos. Todo
eso se cae si al final nadie responde por el texto.

Un medio que firma con su propio nombre le pide al lector que confíe en una
entidad. Una persona que firma se hace responsable: si un dato está mal, hay a
quién reclamarle, y esa persona tiene algo que perder. Por eso **Mistorias es la
publicación, no el autor**.

De ahí salen dos reglas:

- Ninguna historia firma con el nombre del sitio, ni con un colectivo que no
  exista. Un «Equipo» que en realidad es una sola persona es una ficción, y la
  nota justo el lector más atento.
- Una inteligencia artificial **no** aparece como autora. No puede responder por
  un dato mal citado, no tiene reputación que perder y no se le puede reclamar
  nada. Que haya participado se declara aparte (§4).

## 2. Qué se le pide a quien firma

Poco, y por una razón concreta: **todo lo que se publica es permanente**. El
repositorio de contenido es público y su historial no se reescribe, así que cada
dato que se pide es un dato que después no se puede devolver.

La ficha lleva:

- **Nombre** con el que firma.
- **Una línea** que se muestra al pie de cada historia suya.
- **Una biografía corta**, que ella misma redacta, con dos cosas: por qué le
  importa el tema, y algo de ella como persona.
- **Un enlace de verificación, opcional.**

El vínculo con el tema es lo que más confianza da y lo que menos expone: «mi
familia es de aquí», «estudié en colegio público», «enseño en este distrito». Lo
personal humaniza y va en dosis chica. Ninguna de las dos cosas necesita hablar
del trabajo de nadie.

## 3. Qué no se pide, nunca

- **Correo personal.** Ni en la ficha ni en ninguna parte del sitio. Un correo
  es permanente, contactable, y sobre todo es una llave de correlación: enlaza a
  esa persona con todas sus otras cuentas. El contacto del sitio es
  institucional.
- **Empleador o cargo.** Mistorias es un proyecto personal y no debe poder
  leerse como el trabajo de nadie. Además, la credibilidad de quien escribe acá
  no viene de su empleo.
- **Dirección, ciudad exacta ni datos de ubicación fina.**
- **Foto**, salvo que la persona insista. Humaniza, pero es lo que más expone en
  búsquedas y lo que menos aporta para evaluar una historia.

### El enlace de verificación

Cuando alguien quiere que se pueda comprobar que existe, el enlace apunta a un
perfil **que esa persona ya mantiene por su cuenta**: sus redes, su web, la
página de su institución.

Esa condición no es un detalle. Un perfil propio lo puede borrar o cambiar ella
cuando quiera, sin pedirle permiso a nadie. Lo que Mistorias guarda es una URL,
no su contenido. Es la única forma de dar verificación sin publicar algo que
después no se pueda retirar.

Y conviene decirlo con precisión: **ninguna ficha prueba que alguien existe.** Lo
que el lector evalúa es que *alguien responde*. Un periódico no publica el
documento de identidad de su columnista; pone su propio nombre en juego. Acá es
igual: Mistorias publicó, Mistorias responde.

## 4. Cómo se declara el uso de inteligencia artificial

Se usa, así que se dice. Cada historia declara al pie una de tres etiquetas:

| Etiqueta | Cuándo |
|----------|--------|
| `escrito-por-persona` | La IA no tocó el texto. |
| `editado-con-ia` | La persona escribió el cuerpo; la IA corrigió, conectó ideas y sugirió cambios que esa persona aceptó o descartó. |
| `escrito-con-ia` | La IA reunió las noticias y redactó; la persona definió el encargo, ajustó el texto, revisó las fuentes y decide publicarlo. |

Tres decisiones detrás de esto:

- **Va por historia, no por autor.** El reparto cambia: la misma persona puede
  escribir una entera y dirigir la siguiente. Una declaración única en «Acerca
  de» sería falsa en cuanto una historia se aparte del promedio.
- **No es un porcentaje.** «Mitad y mitad» no le sirve a nadie, porque no dice
  *qué* mitad. Una etiqueta de un conjunto cerrado sí le dice al lector cómo
  leer lo que tiene delante.
- **Es una etiqueta, no un cuestionario.** A quien colabora se le pide elegir
  una de tres, no narrar su proceso. La transparencia no debe costar tanto que
  la gente deje de colaborar.

Ninguna de las tres resta mérito, y por eso se declaran las tres —incluida la
que dice que no hubo IA—: si solo se marcara el uso de IA, la etiqueta se leería
como una advertencia y no como información.

## 5. Qué se le promete a quien colabora

Se promete lo que se puede cumplir, y se dice antes y no después:

> Podemos quitar tu ficha del sitio en un día. **No podemos borrarla del
> historial de Git**: el repositorio es público y lo que ya se publicó se puede
> haber clonado. Es como un periódico impreso: se deja de imprimir, no se
> recogen los ejemplares que ya circulan. Por eso te pedimos tan poco.

La consecuencia práctica es la regla que ordena todo este documento: **la forma
de proteger a quien colabora no es prometerle un borrado, es pedirle menos.**

Para pedir que se quite algo, `support@mistorias.pe`.

## 6. Antes de publicar la primera historia de alguien

- [ ] Su ficha existe y la redactó esa persona, no el equipo.
- [ ] La bio dice por qué le importa el tema; no menciona su empleo ni su cargo.
- [ ] No hay correo, dirección ni foto no pedida.
- [ ] Si hay enlace, apunta a un perfil público que ella controla.
- [ ] Se le dijo, con estas palabras, que el historial es permanente.
- [ ] La historia declara su etiqueta de autoría, elegida por lo que de verdad
      pasó al escribirla.
