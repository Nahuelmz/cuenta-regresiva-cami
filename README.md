# Faltan… para volver a ver a Cami ♥

Una cuenta regresiva hasta el reencuentro: **miércoles 1 de julio, 14:30 (hora de Argentina)**.

## Verla en tu compu

Doble clic en `index.html` y listo. Funciona offline.

## Las fotos (una por día)

La página muestra **una foto por día, en orden**: la primera de la lista el
primer día (18/6), la segunda el 19/6, y así hasta el reencuentro. El cambio
ocurre a la medianoche de Argentina, así vos (de viaje) y Cami ven siempre la
misma foto el mismo día. Al llegar al final, queda fija en la última.

Para cargarlas:

1. Copiá todas tus fotos a la carpeta `photos/`.
2. Abrí `index.html` y buscá el bloque `const PHOTOS = [`.
3. Sumá la ruta de cada foto:

```js
const PHOTOS = [
  "photos/foto1.jpg",
  "photos/foto2.jpg",
  "photos/foto3.jpg",
  // ...todas las que quieras
];
```

Si la lista está vacía, se muestra un placeholder con un corazón.

## (Opcional) Barra de progreso del viaje

Si querés ver "qué tanto falta" como una barrita que se va llenando, completá `TRIP_START`
con el día que arrancaste el viaje:

```js
const TRIP_START = new Date("2026-06-03T10:00:00-03:00");
```

Dejala en `null` para ocultarla.

## Subirla online (para que Cami la vea)

Es un sitio estático, así que cualquiera de estas sirve y son gratis:

- **Netlify Drop** → entrá a https://app.netlify.com/drop y arrastrá la carpeta `cuenta-regresiva-cami`. Te da un link al toque.
- **GitHub Pages** → subí la carpeta a un repo y activá Pages sobre la rama `main`.

> La fecha objetivo usa el huso de Argentina (`-03:00`), así que el contador es correcto
> sin importar desde qué país o dispositivo se abra. 🇦🇷
