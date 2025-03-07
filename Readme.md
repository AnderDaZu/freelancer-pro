# Formulario

## Etiqueta Fieldset

En HTML, la etiqueta ***fieldset*** se usa dentro de un formulario ***form*** para agrupar visualmente elementos 
relacionados. Su propósito es mejorar la organización y la accesibilidad del formulario, facilitando 
la comprensión del usuario.

### 📌 Uso de **fieldset**

- Agrupa campos relacionados en un formulario.
- Mejora la organización y la estructura visual.
- Se usa junto con ***legend*** para proporcionar un título al grupo.

```html
<form>
    <fieldset>
        <legend>Información Personal</legend>

        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre">

        <label for="email">Correo Electrónico:</label>
        <input type="email" id="email" name="email">
    </fieldset>

    <fieldset>
        <legend>Detalles de Cuenta</legend>

        <label for="usuario">Usuario:</label>
        <input type="text" id="usuario" name="usuario">

        <label for="password">Contraseña:</label>
        <input type="password" id="password" name="password">
    </fieldset>

    <button type="submit">Enviar</button>
</form>
```

✅ Beneficios de usar ***fieldset***

✔ Organiza mejor los formularios largos.

✔ Mejora la accesibilidad y experiencia del usuario.

✔ Facilita la lectura y navegación.

---

# Preload

Preload dentro de un <link> se usa para cargar recursos de manera anticipada y mejorar el rendimiento de la página 
web. Es útil cuando se sabe que un recurso será necesario pronto, pero el navegador normalmente no lo cargaría de inmediato.

## 📌 ¿Para qué sirve preload?

- Optimizar la carga de la página: Permite cargar archivos antes de que se necesiten, reduciendo el tiempo de espera.
- Evitar bloqueos en la renderización: Recursos críticos, como fuentes o scripts, se pueden cargar antes para evitar retrasos.
- Mejorar la experiencia del usuario: Especialmente útil para imágenes grandes, videos, estilos CSS y fuentes web.

## ⚠ Importante
- No usar preload en exceso, solo en recursos críticos.
- Asegurarse de que los archivos sean realmente necesarios; de lo contrario, puede desperdiciar ancho de banda.
- Combinar preload con async y defer para optimizar scripts JavaScript.

