# EPE — Plataforma de Gestión RSE

**Ética Profesional Empresarial · Plataforma Web de Responsabilidad Social Empresarial**

Herramienta web para que las organizaciones gestionen de forma integral su estrategia de RSE, alineada a los marcos internacionales **ISO 26000**, **ODS / Agenda 2030**, **SDG Compass** y **Doble Materialidad GRI**.

🌐 **[Acceder a la plataforma →](https://mmg15.github.io/EPE-EticaProfesionalEmpresarial/)**

---

## ¿Qué es?

La plataforma EPE permite a empresas de cualquier tamaño definir, gestionar y comunicar su estrategia de RSE a través de tres módulos secuenciales:

| Módulo | Nombre | Descripción |
|--------|--------|-------------|
| **1** | Compromiso con la RSE | Declaración de Misión, Visión y Valores organizacionales |
| **2** | Análisis de Stakeholders | Mapeo e identificación de partes interesadas con matriz influencia × interés |
| **3** | Actividades por Stakeholders | Registro de programas, proyectos, presupuestos e indicadores RSE vinculados a ODS |

### Marcos de referencia

- **ISO 26000** — 7 materias fundamentales y gobernanza organizacional
- **ODS / Agenda 2030** — Vinculación de actividades a los 17 Objetivos de Desarrollo Sostenible
- **SDG Compass** — Flujo de 5 pasos: entender, priorizar, objetivos, integrar, reportar
- **Doble Materialidad GRI** — Perspectiva de impacto y financiera en el análisis de asuntos

### Características técnicas

- **Sin instalación** — Un solo archivo HTML, se abre directo en el navegador
- **Sin servidor** — Funciona 100% del lado del cliente
- **Persistencia local** — Los datos se guardan automáticamente en `localStorage`
- **Exportación** — Descarga de todos los datos en formato JSON
- **Resumen imprimible** — Vista consolidada de los 3 módulos lista para imprimir o exportar a PDF

---

## Cómo usar la plataforma

> 🌐 **Accedé desde tu navegador en: [https://mmg15.github.io/EPE-EticaProfesionalEmpresarial/](https://mmg15.github.io/EPE-EticaProfesionalEmpresarial/)**

### Paso 1 — Configuración inicial

Al ingresar por primera vez verás la pantalla de **Configuración**.

1. Completá el **nombre de tu empresa** (campo obligatorio)
2. Opcionalmente ingresá el sector/industria y el tamaño de la organización
3. Hacé clic en **"Guardar y comenzar"**

El nombre de la empresa aparecerá en el panel lateral durante toda la sesión.

---

### Paso 2 — Módulo 1: Compromiso con la RSE

En esta sección declarás la identidad y el compromiso de tu organización.

1. **Misión** — Escribí el propósito central de tu empresa (campo obligatorio)
2. **Visión** — Describí el estado futuro al que aspira la organización (campo obligatorio)
3. **Valores** — Escribí cada valor y presioná **Enter** para agregarlo como etiqueta. Podés agregar todos los que necesites. (mínimo 1)
4. Hacé clic en **"Guardar y continuar"** para avanzar al Módulo 2

> 💡 Podés guardar un borrador en cualquier momento con el botón **"Guardar borrador"** y retomar más tarde.

---

### Paso 3 — Módulo 2: Análisis de Stakeholders

Mapeá todas las partes interesadas de tu organización.

**Stakeholders precargados**

La plataforma incluye 6 stakeholders primarios predefinidos según ISO 26000:
- Propietarios / Accionistas
- Gerencia
- Empleados
- Clientes
- Proveedores
- Medio Ambiente

Podés **editar** cualquiera de ellos haciendo clic en ✏️.

**Agregar stakeholders secundarios**

1. Hacé clic en **"+ Agregar"**
2. Completá los campos: Nombre, Tipo, Nivel de influencia (1-5), Nivel de interés (1-5), Expectativas y Canal de comunicación
3. Guardá el stakeholder

**Matriz Influencia × Interés**

Al pie del módulo se genera automáticamente una matriz que clasifica a cada stakeholder en uno de los 4 cuadrantes:

| Cuadrante | Estrategia |
|-----------|------------|
| Alta influencia + Alto interés | Gestionar de cerca |
| Alta influencia + Bajo interés | Mantener satisfechos |
| Baja influencia + Alto interés | Mantener informados |
| Baja influencia + Bajo interés | Monitorear |

---

### Paso 4 — Módulo 3: Actividades por Stakeholders

Registrá los programas y proyectos RSE de tu organización.

1. Hacé clic en **"+ Agregar actividad"**
2. Completá los campos:
   - **Programa** — Nombre de la iniciativa macro (ej: *Programa de Empleo Joven 2025*)
   - **Proyecto / Acción** — Acción concreta dentro del programa
   - **Objetivos** — Descripción de los objetivos del proyecto
   - **Presupuesto** — Monto asignado en ARS (solo numérico)
   - **Indicador / KPI** — Métrica de seguimiento (ej: *% empleados capacitados*)
   - **Stakeholders vinculados** — Seleccioná uno o más del Módulo 2
   - **ODS vinculados** — Seleccioná los Objetivos de Desarrollo Sostenible relacionados
3. Guardá la actividad

**Filtrar actividades**

Usá el selector **"Filtrar por stakeholder"** para ver solo las actividades asociadas a una parte interesada específica.

---

### Paso 5 — Resumen y exportación

Una vez completados los módulos tenés dos opciones:

- **📄 Ver resumen** — Abre una vista consolidada con los 3 módulos. Desde ahí podés imprimir o generar un PDF con `Ctrl+P`
- **↓ Exportar JSON** — Descarga todos los datos en formato JSON (útil para backup o integración futura con un backend)

---

## Datos y privacidad

Todos los datos ingresados se almacenan **únicamente en tu navegador** (`localStorage`). No se envía nada a ningún servidor. Si limpiás el caché del navegador o usás el botón **"↺ Reiniciar"**, los datos se eliminarán.

Para no perder el trabajo, usá **"↓ Exportar JSON"** como respaldo.

---

## Stack tecnológico

| Capa | Tecnología |
|------|------------|
| Frontend | HTML5 + CSS3 + JavaScript (vanilla) |
| Persistencia | `localStorage` del navegador |
| Hosting | GitHub Pages |
| Backend / Base de datos | — (MVP sin backend) |

La arquitectura productiva propuesta en los requerimientos es **React + .NET (C#) + MariaDB/SQL Server + MongoDB**.

---

## Estructura del repositorio

```
EPE-EticaProfesionalEmpresarial/
├── index.html   # Aplicación completa (single-file)
└── README.md
```

---

## Contribuir

1. Cloná el repositorio: `git clone https://github.com/MMG15/EPE-EticaProfesionalEmpresarial.git`
2. Realizá tus cambios en `index.html`
3. Hacé commit y push a `main`

Los cambios en `main` se reflejan automáticamente en GitHub Pages en 1-2 minutos.

---

*Proyecto EPE — Versión 1.0 MVP · Junio 2025*
