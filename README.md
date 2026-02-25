# Formateador de Medicación MUP

## Descripción
Esta herramienta facilita la extracción y formateo de la medicación desde el sistema MUP (Módulo Único de Prescripción) para generar un texto limpio y estructurado que puede ser copiado a otros sistemas o documentos clínicos.

## Características Principales
- **Extracción Automática**: Transforma el código HTML copiado del MUP en una lista legible de fármacos con su dosis y posología.
- **Formateo Inteligente**: Simplifica unidades (ej. "ui", "mcg", "mg", "ml") de forma automática.
- **Barra Lateral Interactiva (Checklist)**: Todos los fármacos extraídos se muestran en una barra lateral derecha. Puedes desmarcarlos individualmente para omitirlos del texto final a copiar.
- **Omitir Accesorios**: Una casilla (marcada por defecto) permite filtrar productos sanitarios que no sean medicación estricta (gasas, bolsas, sondas, parches, etc.).

## Instrucciones de Uso

1. **Copiar del MUP**:
   - Haz clic derecho o secundario fuera de la tabla de medicación en el MUP y selecciona "Inspeccionar".
   - Localiza la primera línea que contiene la tabla (normalmente el contenedor HTML principal de la misma) y cópiala con `Ctrl+C` o desde el menú de opciones del click derecho ("Copiar elemento").

2. **Pegar en la Herramienta**:
   - Pulsa el botón principal **"Pegar Portapapeles"** o presiona `Ctrl+V` dentro del área de texto grande.
   - El sistema procesará el texto automáticamente en cuanto haya contenido válido.

3. **Revisar y Filtrar (Nueva Barra Lateral)**:
   - Revisa la barra lateral titulada **"Lista a copiar"**. 
   - Desmarca la casilla junto a cualquier fármaco que no desees incluir en el resultado final. El texto de abajo se actualizará en tiempo real.
   
4. **Copiar Resultado**:
   - Una vez comprobado, presiona **"Copiar contenido"** para llevarte el listado de fármacos formateado y listo para pegar en el historial del paciente.

## Desarrollo
El proyecto consiste en un archivo `index.html` que contiene la interfaz y la lógica de JavaScript para parsear el DOM del MUP.
Los scripts pueden ejecutarse de manera enteramente local sin necesidad de un servidor externo (excepto las librerías CDN como Bootstrap o Firebase analytics).

## Licencia
This work is licensed under a Creative Commons Attribution-NonCommercial 4.0 International License.
