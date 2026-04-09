# ITPro Storefront B (Template Demo)
**Catálogo + Carrito + Pedido por WhatsApp** (sin pagos, sin panel administrable)

## Objetivo
Este repositorio es una **plantilla base reutilizable** (más completa que la A) para negocios de ropa/accesorios que necesitan:
- navegación tipo tienda,
- **carrito** para reunir productos,
- y un flujo de pedido que termina en **WhatsApp**.

Sigue siendo una tienda ligera: **no hay pagos en línea** ni panel administrable.

---

## Alcance (Qué incluye)
### Páginas / secciones (MVP)
- Todo lo de **Storefront A**
- **Carrito**
- **Resumen de pedido**
- CTA final: **“Enviar pedido por WhatsApp”**

### Carrito (definición exacta)
Incluye:
- Agregar/eliminar productos
- Ajustar cantidad
- Subtotal (y notas simples si aplica)
- Persistencia básica (p. ej. mantener carrito durante sesión) — *detalles técnicos TBD*

No incluye:
- Cálculo automático de envío
- Impuestos avanzados
- Cupones / promociones complejas
- Inventario real / stock sincronizado

### Flujo de pedido por WhatsApp
- El usuario arma su carrito
- Generamos un mensaje con:
  - Lista de productos (nombre + cantidad + precio)
  - Subtotal
  - Datos opcionales (nombre del cliente, dirección, notas) **si se habilita**
- Botón final: **Enviar pedido por WhatsApp**

---

## Personalización por cliente
Todo lo de A +:
- Ajustes del mensaje de WhatsApp (formato, campos incluidos)
- Reglas simples (p. ej. mostrar/ocultar campos del formulario previo al envío)

---

## Fuera de alcance (Qué NO incluye)
Para mantenerlo como plantilla “B” y no convertirlo en “C”, **no incluye**:
- ❌ Pagos en línea (Stripe, MercadoPago, PayPal, etc.)
- ❌ Panel administrable / CMS
- ❌ Órdenes guardadas en un sistema
- ❌ Cuentas de usuario / historial de compras
- ❌ Integraciones de envío e inventario (automáticas)

> Si el cliente necesita pagos/admin/órdenes, eso es una **fase superior**.

---

## Principios de la plantilla
- **B = A + carrito + pedido por WhatsApp**
- **Sin pagos, sin panel**
- Modular, rebrandable y repetible
- Alcance claro para poder cotizar/entregar rápido

---

## Estado del proyecto
- **Estatus:** WIP (en construcción)
- **Meta MVP:** demo completa con carrito + WhatsApp order.

---

## Cómo usar este repo
### Como plantilla
1. Marcar este repo como **Template Repository** en GitHub.
2. Crear un nuevo repo desde esta plantilla para un cliente o demo.
3. Personalizar branding + contenido + productos + formato de pedido.

### Ejecución local / Deploy
> **TBD** (definiremos stack, scripts y proceso de deployment cuando arranquemos la implementación).

---

## Definición de “MVP listo”
Se considera listo cuando:
- El sitio es navegable (Home → Categorías → Producto → Carrito).
- El carrito funciona (agrega/elimina/cantidades).
- “Enviar pedido por WhatsApp” genera un mensaje correcto y abre WhatsApp.
- Responsive correcto.
- Data mock suficiente (mín. 10–20 productos).

---

## Roadmap (alto nivel)
- [ ] Estructura base del sitio (layout + navegación)
- [ ] Home modular (secciones configurables)
- [ ] Catálogo + filtros básicos (si aplica)
- [ ] Página de producto + Add to Cart
- [ ] Carrito + resumen de pedido
- [ ] Generación del mensaje WhatsApp (carrito)
- [ ] Config de branding (theme) y contenido
- [ ] Deploy demo (link público) — TBD
