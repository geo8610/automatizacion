---
name: evaluar-candidatos-puestos
description: Compara un grupo de perfiles de candidatos en PDF con exactamente dos descripciones de puesto en PDF, clasifica cada perfil como puesto A, puesto B, ambos o ninguno, genera una lista priorizada para revision humana y publica un reporte en Notion mediante MCP. Usar cuando el usuario entregue curriculums, hojas de vida o perfiles y dos vacantes, especialmente para contratacion remota desde Latinoamerica.
---

# Evaluar candidatos para dos puestos

Analizar evidencia laboral explicita y preparar una recomendacion trazable para revision humana. No tomar una decision final de contratacion.

## Datos necesarios

Solicitar o localizar:

- Una carpeta o lista con los perfiles PDF.
- Exactamente dos descripciones de puesto PDF.
- El destino de Notion. Si no se indica, crear una pagina privada nueva.
- Criterios adicionales relacionados directamente con el trabajo, si existen.

Aceptar cualquier cantidad razonable de candidatos; no limitar el proceso a 30.

## Flujo

1. Inventariar todos los PDFs y confirmar cuantos perfiles y puestos se encontraron.
2. Extraer el texto de cada PDF con las herramientas disponibles. Si un archivo es escaneado, usar lectura visual u OCR. Marcar como `No legible` cualquier archivo que no pueda revisarse; no inventar contenido.
3. Separar requisitos de cada puesto en indispensables, deseables, responsabilidades, experiencia, idioma, horario, ubicacion y permiso laboral.
4. Evaluar cada candidato por separado contra ambos puestos usando [rubrica.md](references/rubrica.md).
5. Clasificar cada candidato como `Puesto A`, `Puesto B`, `Ambos`, `Ninguno` o `Informacion insuficiente`.
6. Ordenar a quienes conviene contactar usando la puntuacion laboral, los requisitos indispensables y la solidez de la evidencia.
7. Revisar nombres, cifras, evidencia y posibles contradicciones.
8. Preparar el reporte siguiendo [reporte-notion.md](references/reporte-notion.md).
9. Publicar el reporte mediante el MCP oficial de Notion.
10. Leer la pagina publicada para verificarla y devolver su enlace.

## Reglas de evaluacion

- Usar solamente datos relacionados con el trabajo y presentes en los documentos.
- Tratar la disponibilidad para trabajar desde Latinoamerica como condicion laboral valida cuando corresponda.
- No usar ni inferir nacionalidad, raza, origen etnico, edad, genero, estado civil, religion, discapacidad, fotografia, orientacion sexual, embarazo, salud u otros datos personales sensibles.
- No asumir ubicacion, permiso laboral, idiomas ni disponibilidad. Marcarlos como `Por confirmar`.
- No favorecer a una persona por el estilo del CV, universidad, prestigio de una empresa o palabras clave aisladas.
- Aplicar la misma rubrica a todos los candidatos.
- Explicar cada recomendacion con evidencia breve.
- Mostrar requisitos indispensables ausentes y datos faltantes.
- Mantener empates o priorizar mejor evidencia, nunca datos personales.
- Presentar el resultado como recomendacion para revision humana.

## Publicacion en Notion

- Usar el servidor oficial `https://mcp.notion.com/mcp`.
- Si falta autenticacion, pedir que conecten Notion y continuar despues.
- Si se entrega una pagina o base de datos, leer primero su estructura y no borrar contenido.
- Si no hay destino, crear una pagina privada titulada `Evaluacion de candidatos - A vs B - AAAA-MM-DD`.
- No publicar los PDFs ni datos de contacto completos.

## Control final

Verificar que:

- todos los candidatos aparecen una sola vez;
- ambos puestos fueron evaluados para cada persona;
- categoria, puntuacion y prioridad son coherentes;
- los datos faltantes estan visibles;
- no se usaron caracteristicas personales protegidas;
- el reporte indica fecha, cantidad de perfiles y archivos no legibles.

