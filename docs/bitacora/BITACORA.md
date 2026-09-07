# 📖 Bitácora del Proyecto

## Sistema de Ventas de Indumentaria

Esta bitácora registra el proceso de desarrollo del proyecto, incluyendo decisiones, avances, documentación, actividades solicitadas por las distintas materias, problemas encontrados y cambios realizados.

---

## 📅 07/09/2026

### Inicio del versionado del proyecto

Se creó el repositorio Git del proyecto **Sistema de Ventas de Indumentaria** y se vinculó con un repositorio remoto en GitHub.

Se definió una estructura inicial de carpetas:

* `backend/`: código correspondiente al backend.
* `database/`: archivos relacionados con la base de datos.
* `docs/`: documentación del proyecto.
* `src/`: código fuente.
* `tests/`: pruebas del sistema.

Se realizó el primer commit:

`chore: creacion de la estructura inicial del proyecto`

### Trabajo de funcionalidades

Se crearon las ramas:

* `feature/productos`
* `feature/clientes`

En `feature/productos` se desarrolló la estructura inicial del módulo de productos y sus operaciones previstas.

En `feature/clientes` se desarrolló la estructura inicial del módulo de clientes y sus operaciones previstas.

Cada funcionalidad fue desarrollada en una rama independiente y documentada mediante varios commits.

### Pull Request

Se creó un Pull Request para integrar la rama `feature/productos` en `main`.

El Pull Request fue revisado y posteriormente integrado correctamente.

### Conflicto controlado

Como parte del TP1 de Versionado y Trabajo Colaborativo, se provocó un conflicto controlado modificando la misma sección del archivo `README.md` desde las ramas `feature/productos` y `feature/clientes`.

El conflicto fue resuelto manualmente combinando los aportes de ambas ramas.

La resolución quedó registrada mediante el commit:

`fix: resolvi conflicto en README integrando productos y clientes`

### Documentación

Se creó el documento:

`docs/TP1-versionado.md`

En él se documentaron las decisiones tomadas sobre la organización de ramas y el proceso de generación y resolución del conflicto.

### Estado actual

El repositorio se encuentra sincronizado con GitHub y la rama `main` no presenta cambios pendientes.

Próximos pasos: continuar con el desarrollo del proyecto y registrar en esta bitácora los avances y decisiones relevantes.
