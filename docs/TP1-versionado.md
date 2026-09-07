# TP1 – Versionado y Trabajo Colaborativo

## 1. Repositorio y estructura del proyecto

Para el desarrollo del proyecto **Sistema de Ventas de Indumentaria** se creó un repositorio Git y se vinculó con un repositorio remoto en GitHub.

La estructura inicial del proyecto quedó organizada de la siguiente manera:

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

La creación de esta estructura fue registrada mediante el primer commit:

`chore: creacion de la estructura inicial del proyecto`

De esta manera, se estableció una base organizada para continuar con el desarrollo del sistema y mantener un historial de cambios.

## 2. Organización de ramas

Para trabajar de manera independiente sobre distintas funcionalidades se utilizaron ramas específicas a partir de `main`.

Las ramas creadas fueron:

* `feature/productos`: destinada al desarrollo del módulo de productos.
* `feature/clientes`: destinada al desarrollo del módulo de clientes.

Esta organización permite separar las funcionalidades y evitar realizar todos los cambios directamente sobre `main`.

### Rama feature/productos

En esta rama se realizaron tres commits:

* `feat: agregue estructura inicial de productos`
* `feat: agregue operaciones de gestion de productos`
* `docs: actualice descripcion del modulo de productos`

En ella se creó el archivo `src/productos.txt`, donde se definieron los datos principales y las operaciones previstas para la gestión de productos.

### Rama feature/clientes

En esta rama también se realizaron tres commits:

* `feat: agregue estructura inicial de clientes`
* `feat: agregue operaciones de gestion de clientes`
* `docs: actualice descripcion del modulo de clientes`

En ella se creó el archivo `src/clientes.txt`, donde se definieron los datos principales y las operaciones previstas para la gestión de clientes.

Se realizaron al menos dos commits por cada rama, permitiendo mantener un historial claro y ordenado de los cambios.

## 3. Integración mediante Pull Request

Una vez finalizado el trabajo correspondiente a `feature/productos`, se creó un **Pull Request** desde esta rama hacia `main`.

El Pull Request se tituló:

**Integración del módulo de productos**

En la descripción se detallaron los cambios realizados y se realizó una revisión básica para comprobar que los cambios correspondieran a la funcionalidad desarrollada.

El Pull Request fue integrado correctamente a `main`, incorporando el archivo `src/productos.txt` y la actualización correspondiente del `README.md`.

## 4. Generación del conflicto

Para cumplir con el requisito de practicar la resolución de conflictos, se generó deliberadamente un conflicto controlado.

El conflicto se produjo porque las ramas `feature/productos` y `feature/clientes` modificaron la misma línea del archivo `README.md`, pero con contenidos diferentes.

La rama `feature/productos` modificó el objetivo del proyecto para mencionar la gestión de productos y el control de stock.

Por otro lado, `feature/clientes` modificó esa misma línea para mencionar la gestión de clientes.

Al intentar integrar `feature/clientes` en `main`, Git detectó que ambas ramas habían modificado la misma sección y mostró un conflicto de contenido en `README.md`.

## 5. Resolución del conflicto

El conflicto fue resuelto manualmente editando el archivo `README.md`.

Se eliminaron las marcas de conflicto generadas por Git y se decidió combinar la información de ambas ramas en una única descripción:

> El proyecto busca brindar una solución para gestionar productos de indumentaria, clientes y ventas de manera organizada, incluyendo el control de stock.

De esta manera, se conservaron los aportes relacionados con productos, clientes y control de stock sin descartar los cambios realizados en ninguna de las dos ramas.

Una vez realizada la modificación, el archivo fue agregado nuevamente al área de preparación mediante:

`git add README.md`

Finalmente, se creó el commit de resolución:

`fix: resolvi conflicto en README integrando productos y clientes`

Este commit permitió finalizar correctamente la integración de la rama `feature/clientes` en `main`.

## 6. Conclusión

El uso de Git y GitHub permitió organizar el desarrollo del proyecto mediante ramas independientes, mantener un historial de cambios descriptivo e integrar funcionalidades de forma controlada.

Además, la creación y resolución de un conflicto permitió practicar una situación habitual en el trabajo colaborativo, comprendiendo cómo Git identifica modificaciones incompatibles y cómo resolverlas manualmente antes de completar una integración.

De esta forma, el proyecto cuenta actualmente con una estructura inicial, dos ramas de funcionalidades trabajadas de manera independiente, un Pull Request integrado y un conflicto correctamente resuelto y documentado.
