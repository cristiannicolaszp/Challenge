# 🏝️ The Archipelago: Private Island Marketplace

## 📌 El Challenge

Bienvenido al Challenge de Frontend para **The Archipelago**, la plataforma de bienes raíces más exclusiva del mundo. Tu misión es construir una interfaz de catálogo para la compraventa de islas privadas, orientada a un público de ultra-lujo.

El objetivo es demostrar tus habilidades en **arquitectura de componentes, manejo de estado, paginación y refinamiento visual (UX/UI)**.

---

## 🎯 Requerimientos del Proyecto

### 1. Listado de Propiedades

* **Consumo de Datos:** Debes utilizar el archivo JSON provisto para generar las cards de forma dinámica.
* **Paginación:** La interfaz debe mostrar exactamente **10 propiedades por página**. Implementar controles de navegación (Anterior/Siguiente).
* **Filtros de Categoría:** Implementar un sistema de filtrado por categoría (Tropical, Mediterranean, Arctic, etc.). Al filtrar, la paginación debe actualizarse acorde a los resultados.
* **Responsive Design:** La grid de propiedades debe ser adaptable:
    * Desktop: 3 o 4 columnas.
    * Tablet: 2 columnas.
    * Mobile: 1 columna.

### 2. Estética "Quiet Luxury"

* **Tipografía:** Se sugiere el uso de fuentes Serif para títulos (ej. *Playfair Display*) y Sans-Serif para datos técnicos (ej. *Montserrat* o *Inter*).
* **Formato de Moneda:** Los precios deben estar formateados correctamente (ej. `450000000` -> `$450,000,000`).
* **Micro-interacciones:** Añadir efectos de hover en las cards (ej. sutil zoom en la imagen) y transiciones suaves al cambiar de página o aplicar filtros.

### 3. Estados de la Aplicación

* **Loading State:** Implementar *Skeleton Screens* para simular la carga de datos (puedes usar un delay artificial de 1s).
* **Empty State:** Mostrar un mensaje elegante si un filtro no arroja resultados.

---

## 🛠️ Stack Tecnológico

* **Framework:** Lo que te sea mas comodo (client-side focus).
* **Estilos:** Tailwind CSS, Styled Components o CSS Modules.
* **Iconos:** Lucide o Phosphor Icons.
* **Animaciones:** Framer Motion o CSS Transitions.

---

## 📂 Estructura Sugerida
```text
├── src/
│   ├── components/
│   │   ├── ui/             # Componentes base (Buttons, Badges)
│   │   ├── IslandCard.jsx
│   │   ├── FilterBar.jsx
│   │   └── Pagination.jsx
│   ├── data/
│   │   └── islands.json    # El dataset de 20 islas
│   ├── hooks/
│   │   └── useIslands.js   # Lógica de paginación y filtrado
│   └── App.jsx


## **Criterios de Evaluación**

1. Calidad de Código: Limpieza, modularización y legibilidad.

2. Fidelidad Visual: Qué tan "premium" se siente la interfaz.

3. Lógica de Paginación: Manejo correcto de los índices del array al cambiar de página.

4. UX: Manejo de estados de carga y errores de forma profesional.