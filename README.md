# MCMI-IV - Cuestionario para enviar por email

Este repo genera un link público tipo https://TU_USUARIO.github.io/mcmi-iv/ que abre el cuestionario directo, sin mostrar código.

## Como desplegar en 2 minutos

1. Creá cuenta en https://github.com
2. New repository -> nombre: `mcmi-iv` -> Public -> Create
3. Upload files -> arrastrá `index.html` de este zip
4. Commit changes
5. Andá a Settings -> Pages -> Build and deployment -> Source: Deploy from a branch -> Branch: main / root -> Save
6. Esperá 1 min y te da el link: `https://TU_USUARIO.github.io/mcmi-iv/`

Ese link es el que mandás por mail al paciente.

## Como cambiar tu email donde llegan respuestas

Abrí `index.html` con Bloc de Notas, buscá:

const EVALUADOR_EMAIL = "aldomontoya09@gmail.com";

Cambialo por tu email.

## Como poner los 195 items reales

Por copyright el archivo trae 15 items demo. Para poner los 195:

1. Generá tu items.json con el extractor de PDF que te di
2. Abrí index.html y reemplazá el array `const ITEMS = [...]` por tus 195 items
3. Hacé commit de nuevo y GitHub Pages se actualiza solo.

El paciente al terminar hace clic en "Enviar por Email al profesional" y te llega a tu Gmail.
