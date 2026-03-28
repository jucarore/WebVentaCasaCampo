# Casa de Campo Sostenible — casacampoalcala.co

## Proyecto

Sitio web de venta de una casa de campo sostenible en Alcalá, Valle del Cauca (Eje Cafetero, Colombia). El objetivo es maximizar la conversión de visitantes en compradores interesados.

## Stack

- HTML5 + CSS3 inline + Vanilla JS — sin frameworks, sin dependencias externas
- Hosting: Netlify (deploy automático al hacer push a `main`)
- Repo: github.com/jucarore/WebVentaCasaCampo
- Dominio: casacampoalcala.co

## Multilenguaje (IMPORTANTE)

El sitio tiene 3 versiones por idioma:

| Idioma | Archivo | Ruta en producción |
|--------|---------|-------------------|
| Español | `index.html` | `/` |
| English | `en/index.html` | `/en/` |
| Français | `fr/index.html` | `/fr/` |

**REGLA CRÍTICA:** Cualquier cambio en CSS, HTML o JavaScript DEBE replicarse en los 3 archivos. No hay templates compartidos — cada archivo es independiente.

- Las rutas de imágenes en ES: `Imagenes/...`
- Las rutas de imágenes en EN y FR: `../Imagenes/...`
- Selector de idioma (ES/EN/FR) en el nav de las 3 versiones
- Meta tags `hreflang` en las 3 páginas

## Estructura

```
index.html                     # Español
en/index.html                  # English
fr/index.html                  # Français
netlify.toml                   # Headers de seguridad (HSTS, CSP, etc.)
Estrategia-Redes-Sociales.md   # Plan de marketing
README.md                      # Documentación
Imagenes/                      # Fotos y videos (compartidos)
```

## Secciones (mismas en los 3 idiomas)

1. Hero — slider 8 fotos + precio + CTA apilados verticalmente
2. Beneficios — 6 cards
3. Ficha técnica — grid de datos
4. Banner solar — estadísticas de sostenibilidad
5. Galería — lightbox, en móvil muestra 6 + botón "ver más"
6. Videos — 3 tours
7. Descripción — detalle de la propiedad
8. Inversión — oportunidad Airbnb
9. Características — 14 features
10. Ubicación — Google Maps
11. Precio — COP y USD
12. Contacto — 3 asesores WhatsApp + formulario

## Responsive

- Mobile-first: secciones 2 columnas se apilan en 1 columna
- Galería: grid 2x2 con máximo 6 fotos + botón expandir
- Banner solar: grid 2x2 en móvil
- Nav: se reorganiza en wrap (logo arriba, links debajo)
- Overflow horizontal bloqueado

## Contactos de la propiedad

- Arturo Cardona: +57 300 7390037
- Luz Stella López: +57 313 7717580
- Liliana Cerón: +57 315 4855410
- Email: casarodriguezarango@gmail.com

## Desarrollo local

```bash
python3 -m http.server 8000
# Abrir http://localhost:8000
```
