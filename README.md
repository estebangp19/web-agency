# 🌐 Web Agency — Desarrollo de Landing Pages

Repositorio de proyectos de desarrollo web para clientes. Especializado en landing pages modernas, rápidas y funcionales usando HTML, Tailwind CSS y APIs externas.

---

## 🗂️ Estructura del repositorio

```
web-agency/
│
├── clientes/                     # Proyectos entregados a clientes
│   ├── vertex-consultoria/       # Consultora de negocios para PyMEs
│   └── fotografo-beisbol/        # Próximo proyecto
│
├── plantillas/                   # Bases reutilizables por tipo de negocio
│   ├── landing-servicios/        # Para consultores, coaches, profesionales
│   ├── landing-fotografo/        # Para fotógrafos y creativos
│   └── landing-ecommerce/        # Para tiendas y productos
│
├── recursos/
│   ├── componentes/              # Secciones reutilizables (heroes, FAQs, forms)
│   └── notas/
│       └── briefing-template.md  # Cuestionario estándar para nuevos clientes
│
└── README.md
```

---

## 🚀 Stack tecnológico

| Tecnología | Uso |
|---|---|
| **HTML5** | Estructura de las páginas |
| **Tailwind CSS** (CDN) | Estilos y diseño responsivo |
| **JavaScript** | Interactividad y animaciones |
| **EmailJS** | Formularios de contacto sin backend |
| **Netlify** | Hosting y deploy |
| **Namecheap** | Registro de dominios |

---

## 📁 Proyectos

### ✅ Vertex Consultoría
> Consultora de negocios para PyMEs mexicanas

- **URL:** [vertex-consultin.netlify.app](https://vertex-consultin.netlify.app)
- **Tipo:** Landing page — Servicios profesionales
- **Secciones:** Hero · Problema · Servicios · Testimonios · FAQ · Contacto
- **Integraciones:** EmailJS (formulario de contacto)
- **Fecha:** Mayo 2025

---

### 🔜 Producer / Beisbol / Deportes en General
> Portafolio y servicios de fotografía deportiva

- **URL:** Próximamente
- **Tipo:** Landing page — Portafolio creativo
- **Estado:** En briefing

---

## 🛠️ Cómo usar una plantilla

1. Copia la carpeta de la plantilla que necesitas
   ```bash
   cp -r plantillas/landing-servicios clientes/nombre-cliente
   ```

2. Abre `index.html` en VS Code y reemplaza el contenido con los datos del cliente

3. Levanta el servidor local para previsualizar
   ```bash
   cd clientes/nombre-cliente
   python -m http.server 8000
   # Abre http://localhost:8000
   ```

4. Configura EmailJS con las keys del proyecto
   ```javascript
   const EMAILJS_PUBLIC_KEY  = "tu_public_key";
   const EMAILJS_SERVICE_ID  = "tu_service_id";
   const EMAILJS_TEMPLATE_ID = "tu_template_id";
   ```

5. Despliega en Netlify arrastrando la carpeta al dashboard

---

## 📋 Flujo de trabajo con clientes

```
1. Briefing          →  Enviar cuestionario al cliente
2. Propuesta         →  Cotización y estructura acordada
3. Desarrollo        →  Construcción en base a plantilla
4. Revisión          →  Preview en Netlify para feedback
5. Ajustes           →  Correcciones según comentarios
6. Entrega           →  Deploy final + dominio del cliente
7. Mantenimiento     →  Soporte mensual opcional
```

---

## 💰 Paquetes de servicio

| Paquete | Incluye | Precio |
|---|---|---|
| **Básico** | Landing page 1 sección, dominio, hosting | $3,000 – $6,000 MXN |
| **Estándar** | 3-5 secciones, formulario, SEO básico | $7,000 – $15,000 MXN |
| **Premium** | + Blog, tienda, integraciones avanzadas | $18,000 – $35,000 MXN |
| **Mantenimiento** | Actualizaciones y soporte mensual | $500 – $1,500 MXN/mes |

---

## 📬 Briefing estándar

El archivo `recursos/notas/briefing-template.md` contiene el cuestionario completo que se envía a cada nuevo cliente antes de iniciar el proyecto. Cubre:

- Información del negocio y diferenciadores
- Público objetivo
- Objetivo de la página (CTA principal)
- Servicios y precios
- Datos de contacto y redes sociales
- Preferencias de diseño y referencias

---

## 📌 Notas de desarrollo

- Tailwind CSS se carga via CDN — suficiente para proyectos de una sola página
- Para proyectos más grandes considerar instalar Tailwind con npm
- EmailJS tiene límite de 200 correos/mes en plan gratuito
- Siempre probar en Netlify antes de conectar dominio del cliente

---

*Desarrollado con HTML, Tailwind CSS y muchas ganas de aprender 🚀*
