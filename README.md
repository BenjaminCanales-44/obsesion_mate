# Obsesión Mate — Tienda online de mates artesanales

🔗 **Demo:** [obsesion-mate.vercel.app](https://obsesion-mate.vercel.app)

Tienda online para un emprendimiento de mates imperiales, camioneros y torpedo, termos, bombillas y materos, con opción de **grabado personalizado**. Los clientes arman su pedido y lo envían por WhatsApp; la dueña gestiona el catálogo desde un panel web.

> Proyecto desarrollado en equipo por **Benjamin Canales** y **[Bryan Piña](https://github.com/Bemol69)**. Participé en el diseño y el desarrollo de funcionalidades.

## ✨ Funcionalidades

- **Catálogo con filtros** por categoría (mates, premium, personalizados, accesorios).
- **Pedido personalizado**: selección de producto, opciones y texto para el grabado, con vista previa del mensaje.
- **Opciones de entrega** (retiro o despacho) con cálculo de fecha estimada.
- **Número de pedido correlativo** y mensaje de WhatsApp generado automáticamente.
- **Horario de atención**: indica si la tienda está abierta o cerrada.
- **Panel de administración (/admin)** con Sveltia CMS para gestionar productos, categorías y fotos.

## 🏗️ Arquitectura

- Sitio estático en **JavaScript vanilla** con los datos en archivos JSON (`data/`).
- **Build en Node.js** (`scripts/build.mjs`) que arma el catálogo, aplica la identidad visual definida en `tienda.config.json` y genera el SEO (Open Graph, Schema.org, sitemap).
- **Publicación continua en Vercel**: cada cambio desde el panel es un commit que se publica automáticamente.

## 🛠️ Tecnologías

JavaScript · HTML5 · CSS3 · Node.js · Sveltia CMS · GitHub · Vercel

## 🚀 Ejecutar localmente

```bash
node scripts/build.mjs
npx serve dist
```
