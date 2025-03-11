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

---

# Selectores

## Selector de Elemento

Seleccionará uno o todos los elementos en base a la etiqueta

```css
p {
    color: blue;
}
```

## Selector de Clase

Una clase se puede crear multiples veces (es reutilizable) e inicia con un punto.

```css
.cliente {
    color: blue;
}
```

## Selector de ID

Se puede tener múltiples ID's por página pero sus nombres no deben repetirse más de una vez por página.

```css
#cliente {
    color: blue;
}
```

## Selector de Atributo

Selecciona elementos basado en algún atributo que tenga.

```css
[src="logo.jpg"] {
    color: blue;
}
```

## Combinación de Descendentes

Selecciona los elementos hijos cuyo padre sea una clase (o ID) en especifico

```css
.cliente .nombre {
    color: blue;
}
```

## Todos los Hijos

Aplica la siguiente regla para todos los párrafos hijos

```css
.cliente > p {
    color: blue;
}
```

---

# Especificidad

La especificidad en CSS es un concepto clave que determina qué reglas de estilo se aplican cuando 
hay varias que podrían afectar el mismo elemento.

📌 ¿Qué es la especificidad en CSS?

La especificidad es un valor numérico que CSS asigna a los selectores para decidir cuál tiene más peso 
cuando hay conflictos de estilos. Mientras mayor sea la especificidad, más prioridad tendrá la regla de CSS.


| Tipo de Selector | Valor Numérico |
|:----------------:|:--------------:|
| Estilos en línea (style="") | 1000 |
| Selectores de ID (#mi-id)	| 100 |
| Selectores de Clase, Atributo y Pseudo-clases (.mi-clase, [type="text"], :hover) | 10 |
| Selectores de Elemento y Pseudo-elementos (h1, p, ::before) | 1 |
| Selector universal (*) y combinadores (>, +, ~ etc.) | 0 |

📌 Regla general: Cuanto más específico sea el selector, más prioridad tiene.

---

# Pseudoselectores
:root -> hace referencia al elemento raiz del documento html 

"Se usa principalmente para definir variables CSS globales y hacer que 
los estilos sean más fáciles de gestionar".

1. 🔥 ¿Cuál es la diferencia entre :root y html?

    Ambos seleccionan el mismo elemento (<html>), pero :root tiene mayor especificidad que html.

2. 🚀 Ventajas de usar :root

    - ✅ Permite crear variables CSS globales.
    - ✅ Hace que los estilos sean más fáciles de modificar y mantener.
    - ✅ Tiene mayor especificidad que html, útil cuando queremos que ciertos estilos sean prioritarios.

3. 📌 Conclusión:

    Usamos :root principalmente para definir variables CSS reutilizables en todo el documento y 
    garantizar que tengan una mayor prioridad que los estilos aplicados a html.

---

# Normalize

Normalize.css se usa en los proyectos para:

✅ Eliminar inconsistencias en los estilos predeterminados de los navegadores.
✅ Hacer que los estilos sean más uniformes en distintos navegadores y dispositivos.
✅ Mantener compatibilidad sin eliminar por completo los estilos nativos útiles.

💡 En resumen: Ayuda a que tu sitio web se vea y funcione de manera más consistente en todos los navegadores. 🚀
