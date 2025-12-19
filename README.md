# LEDONET — Sistema Maestro de Gestión Web

Este repositorio define los **estándares**, **plantillas**, **flujos de trabajo** y la **trazabilidad** necesarios para gestionar todos los proyectos web desarrollados por LEDONET.

Su propósito es asegurar que cada web de cliente:
- Tiene un repositorio limpio y versionado.
- Sigue un flujo de ramas coherente (`main`, `staging`, `feature/*`).
- Usa PRs con estructura obligatoria.
- Lleva un histórico claro de qué se despliega, cuándo y por qué.
- Mantiene entornos de staging y producción controlados.
- Cumple las buenas prácticas de UX, SEO, accesibilidad y despliegues.

---

## 📦 Estructura de este repositorio

/docs
├── standards.md
├── workflows.md
├── pr_template.md
├── issue_templates/
│ ├── feature.md
│ ├── bug.md
│ └── client-request.md
/SITES.md


---

## 🚦 Flujo de ramas (obligatorio en todos los proyectos LEDONET)

- `main` → producción  
- `staging` → entorno de pruebas / QA  
- `feature/*` → desarrollo de una funcionalidad o corrección específica  

Todo cambio **debe** pasar por un Pull Request.

---

## 🧪 Checklist de despliegue

Antes de mergear a `main`, verificar:

- Build limpio, sin errores.
- No hay claves o secretos en el código.
- Enlaces principales funcionan (header, footer, CTAs).
- No se rompe la home ni páginas críticas (contacto, checkout si aplica).
- Se ha actualizado el `CHANGELOG.md` o `DEPLOY_LOG.md`.
- Issue asociado cerrado automáticamente vía GitHub Linking.

---

## 🗂 Registro maestro de webs — `SITES.md`

El archivo `SITES.md` contiene la lista completa de todas las webs activas, en desarrollo o en mantenimiento.  
Cada entrada incluye:

- Cliente  
- Dominio producción y staging  
- Repositorio  
- Stack  
- Estado  
- Notas técnicas / legales / SEO  

---

## 🧪 Cómo crear un nuevo proyecto web LEDONET

1. Crear un nuevo repo desde la plantilla LEDONET.
2. Añadir la entrada correspondiente en `SITES.md`.
3. Crear ramas `main` y `staging` si no existen.
4. Preparar primer Issue (“Preparar estructura base del proyecto”).
5. Preparar primer PR.
6. Conectar staging (Vercel u otro hosting) y validar.

---

## 📞 Contacto técnico interno (LEDONET)

Este repositorio sirve como referencia para todos los desarrolladores y colaboradores técnicos que participen en proyectos LEDONET.

---

LEDONET/
│
├── README.md
├── SITES.md
│
├── docs/
│   ├── standards.md
│   ├── workflows.md
│   ├── pr_template.md
│   └── issue_guidelines.md
│
└── .github/
    ├── PULL_REQUEST_TEMPLATE.md
    └── ISSUE_TEMPLATE/
        ├── feature.md
        ├── bug.md
        └── client-request.md
