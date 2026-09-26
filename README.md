# Sitio de Xelvora: Slide Planets

Página del juego, con la de soporte y la de privacidad que pide App Store
Connect. Es HTML estático: no hay que compilar nada, se sube tal cual a GitHub
Pages.

```
index.html       portada del juego
soporte.html     contacto y preguntas frecuentes  -> URL de soporte
privacidad.html  política de privacidad           -> URL de política de privacidad
css/estilo.css   estilos
js/idioma.js     traducción a los seis idiomas del juego
img/             icono y capturas
```

## Publicarlo en GitHub Pages

1. Crea un repositorio público, por ejemplo `xelvora-web`.
2. Sube **el contenido de esta carpeta** en la raíz del repositorio (que
   `index.html` quede arriba del todo, no dentro de otra carpeta).
3. En el repositorio: **Settings → Pages**. En *Source* elige **Deploy from a
   branch**, rama `main` y carpeta `/ (root)`. Guarda.
4. A los dos o tres minutos la web estará en:
   `https://TU-USUARIO.github.io/xelvora-web/`

## Lo que hay que pegar en App Store Connect

- **URL de soporte:** `https://TU-USUARIO.github.io/xelvora-web/soporte.html`
- **URL de la política de privacidad:** `https://TU-USUARIO.github.io/xelvora-web/privacidad.html`
- **URL de marketing** (opcional): `https://TU-USUARIO.github.io/xelvora-web/`

## Lo único que hay que tocar después

En `index.html`, el botón «Descargar en App Store» apunta a `#`. Cuando la app
esté publicada, cambia ese `#` por el enlace de la ficha y borra la línea del
aviso «Próximamente en App Store» (el párrafo con `data-t="prox"`).
