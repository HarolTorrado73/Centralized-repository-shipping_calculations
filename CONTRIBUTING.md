# Guía de contribución

## ¡Bienvenidos contribuidores!

Gracias por considerar contribuir al **repositorio centralizado de cálculos de envío**. Este documento describe las pautas para colaborar en el desarrollo del proyecto de tarifas y cálculos de envío (Shipping Rates and Calculations).

---

## Cómo contribuir

### 1. Hacer un fork del repositorio

- Crea un fork de este repositorio en tu cuenta de GitHub.
- Clona tu fork localmente: `git clone https://github.com/TU-USUARIO/repo-name.git`
- Configura el remoto `upstream`: `git remote add upstream https://github.com/ORIGINAL-OWNER/repo-name.git`

### 2. Crear una rama para tu cambio

- **Nunca** trabajes directamente en `main`.
- Crea una rama descriptiva: `git checkout -b feature/descripcion-corta` o `fix/correccion-bug`.
- Usa nombres claros: `feature/agregar-validacion-peso`, `fix/formato-moneda`, `docs/actualizar-readme`.

### 3. Realizar tus cambios

- Mantén los cambios **enfocados** (una funcionalidad o corrección por rama).
- Sigue el estilo de código existente en el proyecto.
- Añade comentarios donde ayuden a entender la lógica (por ejemplo, en cálculos de costos de envío).

### 4. Commit y mensajes

- Haz commits atómicos (un cambio lógico por commit).
- Usa mensajes claros en presente:  
  - ✅ `Agregar validación de peso negativo`  
  - ✅ `Corregir cálculo de tarifa por kilogramo`  
  - ❌ `cambios` o `fix`

### 5. Sincronizar con upstream

Antes de abrir un Pull Request:

```bash
git fetch upstream
git checkout main
git merge upstream/main
git checkout tu-rama
git merge main
```

### 6. Abrir un Pull Request (PR)

- Ve a tu fork en GitHub y abre un **Pull Request** hacia la rama `main` del repositorio original.
- **Título**: breve y descriptivo (ej: "Añadir validación de entrada para peso").
- **Descripción**: explica qué cambiaste, por qué y cómo se puede probar.
- Marca el PR como listo para revisión cuando termines.

---

## Estilo de código

- Sigue las convenciones del código existente para mantener **consistencia**.
- Usa nombres de variables descriptivos (por ejemplo, `shipping_cost`, `weight_kg`, `rate_per_kg`).
- Indentación y formato uniformes (recomendado: 4 espacios en Python).

---

## Documentación

- Documenta funciones y lógica no obvia con comentarios.
- Actualiza el `README.md` si añades uso nuevo o dependencias.
- En el PR, incluye una **descripción clara** de los cambios para facilitar la revisión.

---

## Pruebas

- Prueba tus cambios **antes** de enviar el PR (por ejemplo, ejecutando el script con distintos pesos y tarifas).
- Si hay tests en el proyecto, asegúrate de que sigan pasando.
- Incluye en la descripción del PR cómo se puede verificar tu cambio (pasos o ejemplos de entrada/salida).

---

## Issue Tracker

- Revisa los **Issues** abiertos antes de empezar; comenta si vas a trabajar en uno para evitar duplicados.
- Si encuentras un bug o tienes una idea, abre un Issue con título y descripción claros.
- Referencia el Issue en tu PR cuando corresponda (ej: "Closes #3").

---

## Revisión de código

- Todas las contribuciones pasan por **code review**.
- Estar abierto a comentarios y sugerencias; los revisores buscan mejorar la calidad y consistencia del código.
- Responde a los comentarios y aplica los cambios solicitados cuando sea razonable.

---

## Resumen rápido para Coursera

Este repositorio aplica un flujo de trabajo colaborativo estándar:

1. **Fork** → **Rama** → **Cambios** → **Commit** → **Pull Request** → **Revisión** → **Merge**.
2. Se prioriza código legible, documentado y probado.
3. Se usa el Issue Tracker para coordinar tareas y el PR para proponer cambios de forma ordenada.

Tu contribución debe seguir estas pautas para mantener la calidad y facilitar la evaluación por pares.

---

¡Gracias por contribuir!
