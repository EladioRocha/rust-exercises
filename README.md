# Rust-Lab

Prácticas de Rust organizadas en dos proyectos Cargo independientes: una aplicación de tareas por consola y un experimento de automatización gráfica.

## Estructura

- [measure-monkey-bot](measure-monkey-bot)
- [todo-app](todo-app)

## Preparación y uso

Para la aplicación de consola: `cd todo-app` y `cargo run`. Para compilar sin ejecutarla: `cargo check`. `measure-monkey-bot/` usa `autogui` y `winapi` y depende de Windows y de las coordenadas de pantalla; revisa su código antes de ejecutarlo.

## Validación y estado

Esta guía se contrastó con el árbol de archivos y los manifiestos del repositorio. No se ha validado una ejecución completa contra servicios externos, bases de datos o hardware. Las versiones y los scripts mostrados describen el código actual; no implican que sus dependencias antiguas sigan siendo compatibles.
