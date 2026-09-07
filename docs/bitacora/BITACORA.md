# Bitácora del Proyecto — Sistema de Gestión de Ventas

Esta bitácora registra la evolución del proyecto **Sistema de Gestión de Ventas**, orientado a la gestión de ventas de un comercio de indumentaria.

El objetivo de la bitácora es documentar el proceso de desarrollo a lo largo del cuatrimestre, incluyendo decisiones, avances, trabajos prácticos, problemas encontrados, soluciones aplicadas y aprendizajes técnicos.

---

## 📅 07/09/2026 — Inicio del versionado y documentación

### Objetivo de la jornada

Durante esta jornada se trabajó en la organización, versionado y documentación inicial del proyecto **Sistema de Gestión de Ventas**, utilizando Git y GitHub.

El objetivo fue comenzar a trabajar con un flujo de desarrollo basado en ramas, commits y Pull Requests, dejando registrados los avances para poder integrar posteriormente las distintas funcionalidades del sistema.

---

## 🗂️ Estructura inicial del proyecto

Se creó el repositorio del proyecto:

**Sistema de Gestión de Ventas**

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

Los principales datos definidos para el módulo fueron:

* Nombre
* Categoría
* Talle
* Precio
* Stock

Las operaciones previstas fueron:

* Registrar producto
* Consultar producto
* Modificar producto
* Actualizar stock

### Rama `feature/clientes`

También se trabajó en una rama independiente para el módulo de clientes.

En esta rama se realizaron los siguientes cambios:

* Se agregó la estructura inicial del módulo de clientes.
* Se definieron los datos principales de los clientes.
* Se agregaron operaciones previstas para la gestión de clientes.
* Se actualizó la descripción del proyecto en el README.

El archivo creado fue:

```text
src/clientes.txt
```

Los principales datos definidos fueron:

* Nombre
* Apellido
* DNI
* Teléfono
* Correo electrónico

Las operaciones previstas fueron:

* Registrar cliente
* Consultar cliente
* Modificar cliente
* Eliminar cliente

---

## 💾 Commits realizados

Se utilizaron commits separados para registrar cada avance y mantener un historial claro del desarrollo.

Entre los commits realizados se encuentran:

```text
feat: agregue estructura inicial de productos
feat: agregue operaciones de gestion de productos
docs: actualice descripcion del modulo de productos
feat: agregue estructura inicial de clientes
feat: agregue operaciones de gestion de clientes
docs: actualice descripcion del modulo de clientes
```

También se realizó un commit inicial para crear la estructura del proyecto:

```text
chore: creacion de la estructura inicial del proyecto
```

Los commits permiten identificar de forma clara qué cambio se realizó en cada momento.

---

## 🔀 Integración mediante Pull Request

Una vez finalizado el trabajo de la rama `feature/productos`, se realizó un **Pull Request** hacia `main`.

El Pull Request permitió revisar los cambios realizados en el módulo antes de integrarlos a la rama principal.

Finalmente, el Pull Request fue revisado e integrado mediante merge a `main`.

De esta manera, el módulo de productos pasó a formar parte del proyecto principal.

---

## ⚠️ Resolución de conflicto

Al intentar integrar posteriormente la rama `feature/clientes` a `main`, se produjo un conflicto en:

```text
README.md
```

El conflicto ocurrió porque tanto `main` como `feature/clientes` habían modificado la misma sección del archivo, específicamente la descripción del objetivo del proyecto.

Git marcó el conflicto para que pudiera resolverse manualmente.

Se decidió conservar e integrar la información correspondiente a los módulos de:

* Productos
* Clientes
* Ventas
* Control de stock

La descripción final quedó orientada al proyecto completo y no únicamente a una funcionalidad específica.

Una vez solucionado el conflicto, se ejecutaron los siguientes comandos:

```bash
git add README.md
git commit -m "fix: resolvi conflicto en README integrando productos y clientes"
git push origin main
```

El conflicto quedó resuelto y la rama `main` pasó a contener los cambios integrados de ambas funcionalidades.

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

Posteriormente fue agregado al repositorio mediante Git.

El commit utilizado fue:

```text
docs: agregue el informe del TP1 de versionado
```

Luego se realizó el `push` hacia GitHub.

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

## 🏗️ 07/09/2026 — Decisión de arquitectura

### Metodología de Sistemas II

Se trabajó sobre la definición de la arquitectura del **Sistema de Gestión de Ventas**.

Se analizaron dos alternativas principales:

1. Arquitectura monolítica en capas.
2. Arquitectura basada en microservicios.

Luego del análisis de los trade-offs, se decidió utilizar una **arquitectura monolítica en capas**, considerando el alcance actual del sistema, el tamaño del equipo y la necesidad de evitar complejidad innecesaria.

La alternativa basada en microservicios se considera técnicamente válida, pero actualmente agregaría complejidad de desarrollo, comunicación, despliegue y mantenimiento que no resulta necesaria para el alcance definido.

La decisión podrá revisarse en el futuro si aumentan significativamente los usuarios, los requerimientos de escalabilidad o la necesidad de desplegar componentes de manera independiente.

La documentación específica de esta decisión se encuentra en:

```text
docs/bitacora/metodologia-sistemas-II/decisiones-arquitectura.md
```

---

## 🎓 07/09/2026 — Programación IV: TP0 y modelo de datos

Como parte de **Programación IV**, se trabajó en el TP0 correspondiente al diseño de la base de datos como fundamento para el futuro backend del proyecto.

En el TP0 se trabajó sobre:

* normalización de bases de datos;
* análisis de 1FN, 2FN y 3FN;
* identificación de anomalías;
* transformación de un modelo UNF hasta 3FN;
* identificación de dependencias;
* definición de entidades;
* definición de claves primarias y foráneas;
* diseño del Diagrama Entidad-Relación;
* análisis de relaciones entre entidades;
* resolución de relaciones N:M mediante una entidad asociativa;
* proyección del modelo hacia SQLAlchemy;
* análisis inicial de esquemas Pydantic;
* propuesta inicial de endpoints REST para el futuro backend.

El modelo final definido para el TP0 cuenta con las siguientes entidades:

1. `CLIENTE`
2. `VENTA`
3. `CATEGORIA`
4. `PRODUCTO`
5. `DETALLE_VENTA`
6. `TELEFONO_CLIENTE`
7. `EMAIL_CLIENTE`
8. `MEDIO_PAGO_VENTA`

Este modelo será tomado como referencia para las próximas etapas del desarrollo del sistema.

La documentación específica del trabajo se encuentra dentro de:

```text
docs/bitacora/programacion-IV/
```

---

## 🔗 Relación entre las materias y el proyecto integrador

El proyecto **Sistema de Gestión de Ventas** será desarrollado progresivamente durante el cuatrimestre.

Los contenidos y trabajos prácticos realizados en las distintas materias podrán incorporarse al repositorio cuando estén relacionados con el proyecto.

De esta manera, los diferentes trabajos no se consideran actividades aisladas, sino partes de un mismo proceso de análisis, diseño, desarrollo y documentación.

Por ejemplo:

* **Programación IV** aporta el diseño y normalización de la base de datos y posteriormente el desarrollo del backend.
* **Metodología de Sistemas II** aporta el análisis y la toma de decisiones relacionadas con la arquitectura del sistema.
* Los contenidos de otras materias podrán incorporarse posteriormente cuando contribuyan al desarrollo del proyecto.

---

## 📌 Estado actual del proyecto

Actualmente el proyecto cuenta con:

* repositorio Git inicializado;
* repositorio remoto en GitHub;
* estructura básica de carpetas;
* documentación inicial;
* módulos preliminares de productos y clientes;
* historial de commits;
* utilización de ramas para separar funcionalidades;
* integración mediante Pull Request;
* resolución de un conflicto de merge;
* documentación del TP1 de versionado;
* definición inicial de la arquitectura;
* modelo de datos normalizado hasta 3FN;
* documentación de trabajos correspondientes a distintas materias;
* bitácora para registrar la evolución del proyecto.

El proyecto se encuentra en una etapa inicial de análisis, diseño y preparación para la implementación.

---

## 🚀 Próximos pasos

Los próximos avances se irán incorporando a esta bitácora a medida que se realicen.

Entre las próximas etapas previstas se encuentran:

* continuar con el desarrollo del proyecto integrador;
* implementar la base de datos;
* comenzar el desarrollo del backend;
* implementar los modelos correspondientes;
* desarrollar los endpoints necesarios;
* incorporar autenticación y gestión de usuarios;
* realizar pruebas;
* documentar los cambios y decisiones importantes;
* integrar progresivamente los contenidos de las distintas materias.

Cada avance significativo deberá quedar registrado en esta bitácora, manteniendo una visión cronológica de la evolución del **Sistema de Gestión de Ventas**.

---

## 📖 Criterio de documentación

La bitácora funcionará como un registro general del proyecto.

Los trabajos extensos o específicos de cada materia se conservarán en documentos independientes dentro de las carpetas correspondientes.

De esta forma:

```text
BITACORA.md
```

contendrá el **resumen cronológico y las decisiones principales**, mientras que los documentos específicos contendrán el desarrollo detallado de cada trabajo práctico.

La documentación se irá actualizando durante el desarrollo del proyecto para conservar evidencia de las decisiones, cambios, problemas, soluciones y aprendizajes obtenidos durante el proceso.
