# Bitácora del Proyecto — Sistema de Ventas de Indumentaria

## 📅 07/09/2026 — Inicio del versionado y documentación

### Objetivo de la jornada

Durante esta jornada se trabajó en la organización, versionado y documentación inicial del proyecto **Sistema de Ventas de Indumentaria**, utilizando Git y GitHub.

El objetivo fue comenzar a trabajar con un flujo de desarrollo basado en ramas, commits y Pull Requests, dejando registrados los avances para poder integrar posteriormente las distintas funcionalidades del sistema.

---

## 🗂️ Estructura inicial del proyecto

Se creó el repositorio del proyecto:

**Sistema de Ventas de Indumentaria**

La estructura inicial quedó organizada de la siguiente manera:

```text
sistema-ventas/
├── backend/
├── database/
├── docs/
├── src/
├── tests/
├── .gitignore
└── README.md
```

El proyecto está orientado a la gestión de ventas de un comercio de indumentaria.

---

## 🌿 Trabajo con ramas

Se trabajó con ramas independientes para separar las funcionalidades del proyecto.

### Rama `feature/productos`

Se creó y desarrolló la rama correspondiente al módulo de productos.

En esta rama se realizaron los siguientes cambios:

* Se agregó la estructura inicial del módulo de productos.
* Se definieron los datos principales de los productos.
* Se agregaron operaciones previstas para la gestión de productos.
* Se actualizó la descripción del proyecto en el README.

El archivo creado fue:

```text
src/productos.txt
```

### Rama `feature/clientes`

También se trabajó en una rama independiente para el módulo de clientes.

En esta rama se realizaron los siguientes cambios:

* Se agregó la estructura inicial del módulo de clientes.
* Se definieron las operaciones previstas para la gestión de clientes.
* Se actualizó la descripción del proyecto en el README.

El archivo creado fue:

```text
src/clientes.txt
```

---

## 💾 Commits realizados

Se utilizaron commits separados para registrar cada avance.

Entre los commits realizados se encuentran:

* `feat: agregue estructura inicial de productos`
* `feat: agregue operaciones de gestion de productos`
* `docs: actualice descripcion del modulo de productos`
* `feat: agregue estructura inicial de clientes`
* `feat: agregue operaciones de gestion de clientes`
* `docs: actualice descripcion del modulo de clientes`

Los commits permiten identificar de forma clara qué cambio se realizó en cada momento.

---

## 🔀 Integración mediante Pull Request

Una vez finalizado el trabajo de la rama `feature/productos`, se realizó un **Pull Request** hacia `main`.

El Pull Request permitió revisar los cambios antes de integrarlos.

Finalmente, el Pull Request fue aprobado e integrado a `main`.

Esto permitió incorporar el módulo de productos al proyecto principal.

---

## ⚠️ Resolución de conflicto

Al intentar integrar posteriormente la rama `feature/clientes` a `main`, se produjo un conflicto en:

```text
README.md
```

El conflicto ocurrió porque tanto `main` como `feature/clientes` habían modificado la misma sección del archivo, específicamente la descripción del objetivo del proyecto.

Git marcó el conflicto para que pudiera resolverse manualmente.

Se decidió conservar e integrar la información correspondiente a ambos módulos:

* productos
* clientes

Una vez solucionado el conflicto, se ejecutó:

```bash
git add README.md
git commit -m "fix: resolvi conflicto en README integrando productos y clientes"
git push origin main
```

El conflicto quedó resuelto y `main` pasó a contener los cambios de ambas funcionalidades.

---

## 📤 Sincronización con GitHub

Luego de realizar las integraciones, se verificó el estado del repositorio mediante:

```bash
git status
```

El resultado final fue:

```text
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

Esto confirmó que la rama local `main` estaba sincronizada con GitHub y que no había cambios pendientes.

---

## 📚 Documentación del TP1 de Versionado

Como parte del trabajo práctico de versionado, se creó el documento:

```text
docs/TP1-versionado.md
```

El documento contiene el informe correspondiente al trabajo realizado con Git y GitHub.

Posteriormente fue agregado al repositorio mediante Git, se creó el commit:

```text
docs: agregue el informe del TP1 de versionado
```

y se realizó el `push` hacia GitHub.

---

## 📝 Inicio de la bitácora

Como siguiente paso se decidió incorporar una bitácora permanente dentro del repositorio.

La bitácora tendrá como objetivo registrar el proceso de desarrollo del proyecto a lo largo del cuatrimestre.

Se documentarán, entre otras cosas:

* avances del proyecto;
* decisiones tomadas;
* cambios importantes;
* trabajos prácticos relacionados;
* documentación solicitada por las distintas materias;
* problemas encontrados y cómo fueron solucionados;
* cambios en el diseño del sistema;
* avances en el backend;
* diseño y modificaciones de la base de datos;
* aprendizajes técnicos;
* integraciones entre contenidos de distintas materias.

La intención es que el repositorio no solamente contenga el código del proyecto, sino que también permita visualizar **cómo fue evolucionando el proyecto desde su planificación hasta su implementación final**.

---

## 🎓 Relación con el Proyecto Integrador

El proyecto **Sistema de Ventas de Indumentaria** será desarrollado progresivamente durante el cuatrimestre.

Los contenidos y trabajos prácticos realizados en las distintas materias podrán incorporarse a este repositorio cuando estén relacionados con el proyecto.

Por ejemplo, en **Programación IV**, el TP0 permitió comenzar a definir el modelo de datos que servirá como base para el futuro backend desarrollado con FastAPI.

En dicho trabajo se realizó:

* investigación sobre normalización;
* análisis de 1FN, 2FN y 3FN;
* identificación de anomalías;
* transformación de un modelo UNF hasta 3FN;
* definición de entidades, PK y FK;
* diseño del DER;
* análisis de relaciones entre entidades;
* proyección del modelo hacia SQLAlchemy;
* análisis de esquemas Pydantic;
* propuesta inicial de endpoints REST.

El modelo final definido en el TP0 cuenta con las siguientes entidades:

1. CLIENTE
2. VENTA
3. CATEGORIA
4. PRODUCTO
5. DETALLE_VENTA
6. TELEFONO_CLIENTE
7. EMAIL_CLIENTE
8. MEDIO_PAGO_VENTA

Este modelo será tomado como referencia para las próximas etapas del desarrollo del sistema.

---

**Estado actual:** proyecto versionado y sincronizado con GitHub.

**Próximo paso:** continuar con el desarrollo del proyecto integrador y registrar en esta bitácora los nuevos avances y trabajos relacionados.
