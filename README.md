# 📝 Notas App con IndexedDB

Este es un prototipo funcional de una aplicación de notas desarrollado como parte del Taller Práctico.

## 🚀 Tecnologías utilizadas

- **Lenguaje:** HTML, JavaScript
- **Librerías/frameworks:** Ninguno
- **Base de datos:** IndexedDB (almacenamiento local del navegador)
- **Servicios de red:** Simulación con `console.log()`

---

## 🎯 ¿Qué hace la aplicación?

- Permite al usuario escribir una nota o recordatorio.
- Guarda cada nota localmente en una base de datos del navegador (IndexedDB).
- Muestra todas las notas guardadas en pantalla automáticamente.
- Simula el envío de cada nota a un servidor REST (consola).

---

## 🛠️ ¿Cómo se guarda la nota localmente?

- Al hacer clic en "Guardar Nota":
  - Se genera un objeto con `id`, `contenido` y `fecha`.
  - Se almacena en una base de datos local llamada `NotasDB` usando IndexedDB.
  - Se muestra inmediatamente en la interfaz.

---

## 🌐 ¿Cómo se simula el envío al servidor?

- Luego de guardar la nota, se llama a una función `enviarAlServidor(nota)`.
- Esta función imprime el contenido JSON de la nota en la consola del navegador:
  ```javascript
  console.log("📤 Simulando envío al servidor REST:", JSON.stringify(nota));

