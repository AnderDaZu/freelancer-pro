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

