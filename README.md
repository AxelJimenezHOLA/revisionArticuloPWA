# Instrucciones para probar `ArticleUploadForm`

## 1. Abrir la aplicación

1. Descarga el archivo `index.html` en tu computadora.
2. Abre el archivo en tu navegador de preferencia.

---

## 2. Subir un artículo

1. En el formulario:
   - Escribe un **Título**.
   - Escribe un **Resumen**.
   - Selecciona un archivo **PDF** desde tu computadora.
2. Haz clic en **"Enviar artículo"**.

---

## 3. Verificar comportamiento esperado

Después de enviar:

- El formulario debe limpiarse automáticamente.
- El artículo debe aparecer en la sección **"Mis artículos"**.
- El estado debe mostrarse como: `Enviado`.
- Debe mostrarse el nombre del archivo seleccionado.

---

## 4. Probar validaciones

Prueba los siguientes casos:

- Intentar enviar sin completar todos los campos → debe mostrar error.
- Intentar subir un archivo que no sea PDF → debe mostrar error.

---

## 5. Probar persistencia (LocalStorage)

1. Recarga la página (F5 o Ctrl + R).
2. Verifica que los artículos siguen apareciendo en la lista.

---

## 6. Verificar datos en LocalStorage (opcional)

En el navegador:

1. Presiona `F12` para abrir DevTools.
2. Ve a la pestaña **Application** (o "Aplicación").
3. Selecciona **Local Storage** → dominio actual.
4. Busca la clave: `articles`.
5. Verifica que contiene los datos en formato JSON.
