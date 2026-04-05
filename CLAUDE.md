# CLAUDE.md — Regalos Navidades

## Proyecto

Web de afiliados de regalos de Navidad. Sitio estático en HTML/CSS desplegado en **GitHub Pages** con dominio personalizado `regalosnavidades.com`.

- Repositorio: `github.com/onejensen/RegalosNavidades`
- Deploy: `git push origin main` → GitHub Pages publica automáticamente en 1-2 minutos

---

## Páginas

| Archivo | URL |
|---|---|
| `index.html` | Inicio |
| `familia.html` | Regalos para la familia |
| `peques.html` | Regalos para niños |
| `pareja.html` | Regalos para tu pareja |
| `para-el.html` | Regalos para hombre |
| `para-ella.html` | Regalos para mujer |
| `economicos.html` | Regalos económicos |

---

## Afiliados

### Amazon
- Tag: `onejensen00-21`
- Formato búsqueda: `https://www.amazon.es/s?k=TERMINO&tag=onejensen00-21`
- Formato categoría: `https://www.amazon.es/b?_encoding=UTF8&tag=onejensen00-21&node=NODEID`

### AliExpress
- **`s.click.aliexpress.com` NO funciona desde España** — el dominio falla con error SSL/conexión.
- Usar links directos de producto con parámetros `pdp_npi` generados desde el portal de afiliados:
  `https://es.aliexpress.com/item/ITEMID.html?pdp_npi=...affd...`
- Estos links se generan visitando el producto en AliExpress con la extensión de Portals activa en Chrome.
- **No usar** el generador de links cortos de Portals para páginas de búsqueda/categoría — no funcionan.

---

## Imágenes

### Imágenes locales (en `/images/`)
- `perfumesmujer.webp` — usada en `para-ella.html` y `pareja.html` para perfumes de mujer
- `perfumeshombre.webp` — usada en `para-el.html` y `pareja.html` para perfumes de hombre
- `regalosninos.webp`, `regalospareja.webp`, `blackfriday.webp`, etc. — heroes de cada página

### Unsplash
- La URL `photo-1588776814546-1ffbb5cb01a5` está caída — **no usar**
- La URL `photo-1523293182086-7651a899d37f` muestra un perfume de hombre (Bleu de Chanel) — no usar para secciones femeninas
- Cuando una imagen de Unsplash falla, reemplazar por la imagen local correspondiente en `/images/`

---

## Estructura de cada página de categoría

```html
<nav class="site-nav"> <!-- nav con enlace activo en color gold -->
<header class="cat-hero"> <!-- hero con imagen de fondo local -->
<main>
  <div class="product-sections-grid container">
    <div class="product-section">
      <h2>Nombre sección</h2>
      <p class="section-desc">Descripción...</p>
      <div class="products-grid">
        <div class="product-card">
          <div class="product-img"><img ...></div>
          <div class="product-body">
            <p class="product-name">...</p>
            <p class="product-price">desde X,XX €</p>
            <div class="product-btns">
              <a class="btn-amazon" ...>Amazon</a>
              <a class="btn-ali" ...>AliExpress</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="seo-text">...</div>
  <section class="section"> <!-- newsletter MailerLite --> </section>
</main>
<footer class="site-footer">...</footer>
```

---

## Analytics y servicios externos

- Google Analytics: `G-V09HTLH00L`
- Beam Analytics: token `f0260c31-1d1d-425e-8122-ad8e67e077c6`
- MailerLite: account `662923`, form `1QvclZ`
- Contacto: `mejoresnavidades@gmail.com`
