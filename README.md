# 🔬 Calculadora de Ciclo de Trabajo - Laboratorio Virtual de Electrónica de Potencia

[![Netlify Status](https://api.netlify.com/api/v1/badges/your-badge-id/deploy-status)](https://app.netlify.com/sites/your-site-name/deploys)
[![HTML](https://img.shields.io/badge/HTML-100%25-orange.svg)](https://github.com/JoseDFabra/calculadora-ciclo-trabajo)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Laboratorio virtual interactivo para el análisis de convertidores de electrónica de potencia. Herramienta educativa que permite calcular el factor de transformación (Md), eficiencia y puntos críticos mediante expresiones personalizables. Desarrollado para estudiantes del ITM.**

## 🚀 Demo en Vivo

🌐 **[Ver Demo](https://calculadora-ciclo-trabajo.netlify.app)** *(Próximamente)*

## 📋 Tabla de Contenidos

- [Características](#-características)
- [Capturas de Pantalla](#-capturas-de-pantalla)
- [Instalación y Uso](#-instalación-y-uso)
- [Despliegue](#-despliegue)
- [Funcionalidades](#-funcionalidades)
- [Tecnologías](#-tecnologías)
- [Contribuir](#-contribuir)
- [Roadmap](#-roadmap)
- [Licencia](#-licencia)
- [Contacto](#-contacto)

## ✨ Características

- 🧮 **Cálculo de Factor de Transformación (Md)** con expresiones personalizables
- ⚡ **Análisis de Eficiencia** en convertidores DC-DC
- 📊 **Visualización Gráfica** interactiva con Chart.js
- 🎯 **Detección Automática** de puntos críticos (máximos y mínimos)
- 🔄 **Dos Modos de Entrada**: Expresión simple o fracción (numerador/denominador)
- 🚀 **Acciones Rápidas** para funciones matemáticas comunes
- 📱 **Diseño Responsive** para móviles y tablets
- 🎨 **Interfaz Moderna** con efectos visuales avanzados
- 🔬 **Herramienta Educativa** diseñada para estudiantes de ingeniería

## 📸 Capturas de Pantalla

### Interfaz Principal
![Interfaz Principal](screenshots/main-interface.png)

### Modo Fracción
![Modo Fracción](screenshots/fraction-mode.png)

### Gráficas Interactivas
![Gráficas](screenshots/charts.png)

## 🛠️ Instalación y Uso

### Opción 1: Uso Directo (Recomendado)
```bash
# Clonar el repositorio
git clone https://github.com/JoseDFabra/calculadora-ciclo-trabajo.git

# Navegar al directorio
cd calculadora-ciclo-trabajo

# Abrir en el navegador
open power_electronics_analyzer.html
```

### Opción 2: Servidor Local
```bash
# Con Python 3
python -m http.server 8000

# Con Node.js (si tienes http-server instalado)
npx http-server

# Luego abrir: http://localhost:8000
```

### Opción 3: Live Server (VS Code)
1. Instala la extensión "Live Server" en VS Code
2. Abre el archivo `power_electronics_analyzer.html`
3. Click derecho → "Open with Live Server"

## 🌐 Despliegue

### Netlify (Recomendado)
1. **Fork** este repositorio
2. Conecta tu cuenta de [Netlify](https://netlify.com) con GitHub
3. Selecciona el repositorio `calculadora-ciclo-trabajo`
4. Configuración de build:
   - **Build command**: *(dejar vacío)*
   - **Publish directory**: `/`
5. ¡Deploy automático! 🚀

### GitHub Pages
1. Ve a **Settings** → **Pages** en tu repositorio
2. Selecciona **Deploy from a branch**
3. Elige **main branch** y **/ (root)**
4. Tu sitio estará disponible en: `https://tu-usuario.github.io/calculadora-ciclo-trabajo`

### Vercel
```bash
# Instalar Vercel CLI
npm i -g vercel

# En el directorio del proyecto
vercel

# Seguir las instrucciones
```

## 🔧 Funcionalidades

### Cálculos Principales
- **Factor de Transformación (Md)**: Análisis de la relación de transformación
- **Eficiencia (η)**: Cálculo de eficiencia del convertidor
- **Puntos Críticos**: Detección automática de máximos y mínimos

### Modos de Entrada
1. **Expresión Simple**: Una sola expresión matemática
2. **Modo Fracción**: Numerador y denominador separados

### Funciones Matemáticas Soportadas
- Trigonométricas: `sin()`, `cos()`, `tan()`
- Exponenciales: `exp()`, `log()`, `sqrt()`
- Operadores: `+`, `-`, `*`, `/`, `^`
- Variables: `D` (duty cycle), `Rl`, `R`

### Visualización
- **Gráfica Md vs D**: Factor de transformación vs ciclo de trabajo
- **Gráfica η vs D**: Eficiencia vs ciclo de trabajo  
- **Gráfica Combinada**: Ambas métricas en una sola vista
- **Puntos críticos marcados** en todas las gráficas

## 🛠️ Tecnologías

- **HTML5**: Estructura semántica
- **CSS3**: Estilos modernos con gradientes y animaciones
- **JavaScript (ES6+)**: Lógica de cálculos y interactividad
- **Chart.js**: Visualización de gráficas interactivas
- **Math.js**: Evaluación segura de expresiones matemáticas

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Este proyecto está diseñado para ser mejorado por la comunidad estudiantil.

### Cómo Contribuir
1. **Fork** el proyecto
2. Crea una **rama** para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. **Commit** tus cambios (`git commit -m 'Agregar nueva funcionalidad'`)
4. **Push** a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un **Pull Request**

### Ideas para Contribuir
- 📊 Nuevos tipos de gráficas
- 🧮 Más funciones matemáticas
- 🎨 Mejoras en la UI/UX
- 📱 Optimizaciones móviles
- 🌍 Internacionalización
- 📚 Más ejemplos educativos
- 🔧 Nuevos tipos de convertidores

### Reportar Bugs
Usa las [Issues](https://github.com/JoseDFabra/calculadora-ciclo-trabajo/issues) para reportar bugs o sugerir mejoras.

## 🗺️ Roadmap

### Versión 2.0 (Próximamente)
- [ ] Soporte para convertidores Buck, Boost, Buck-Boost
- [ ] Análisis de ondulación (ripple)
- [ ] Exportar resultados a PDF
- [ ] Modo oscuro
- [ ] Guardar configuraciones

### Versión 2.1
- [ ] Análisis de estabilidad
- [ ] Simulación temporal
- [ ] Comparación de múltiples configuraciones
- [ ] API REST para integraciones

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.

```
MIT License

Copyright (c) 2024 José D. Fabra

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

## 👨‍🎓 Uso Educativo

Este proyecto fue desarrollado como herramienta educativa para estudiantes de **Ingeniería Electrónica** del **Instituto Tecnológico Metropolitano (ITM)**. 

### Para Estudiantes
- Úsalo para verificar cálculos de tus tareas
- Experimenta con diferentes expresiones
- Visualiza el comportamiento de convertidores
- Aprende sobre puntos críticos y eficiencia

### Para Profesores
- Herramienta de apoyo en clases
- Ejemplos interactivos
- Verificación rápida de resultados
- Fácil de integrar en el currículo

## 📞 Contacto

**José D. Fabra**
- 📧 Email: [josefabra.dev@gmail.com](mailto:josefabra.dev@gmail.com)
- 🐙 GitHub: [@JoseDFabra](https://github.com/JoseDFabra)
- 🏫 Institución: Instituto Tecnológico Metropolitano (ITM)

---

### 🌟 ¿Te gusta el proyecto?

Si este proyecto te ha sido útil, considera:
- ⭐ Darle una **estrella** al repositorio
- 🍴 Hacer un **fork** para tus propias mejoras
- 📢 **Compartirlo** con tus compañeros de clase
- 🐛 **Reportar bugs** o sugerir mejoras

---

**Hecho con ❤️ para la comunidad estudiantil del ITM**
