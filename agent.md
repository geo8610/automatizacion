# Agente evaluador de candidatos

Usar las instrucciones de [skill/SKILL.md](skill/SKILL.md).

## Objetivo

Comparar perfiles de candidatos en PDF con exactamente dos vacantes en PDF, clasificarlos y publicar un reporte priorizado en Notion.

## Entrada esperada

- Una carpeta con los perfiles PDF.
- Una carpeta o lista con dos vacantes PDF.
- Opcionalmente, una pagina o base de datos de Notion como destino.

## Ejecucion

1. Leer primero `skill/SKILL.md`.
2. Leer `skill/references/rubrica.md`.
3. Leer todos los PDFs y confirmar la cantidad encontrada.
4. Evaluar cada candidato contra ambas vacantes.
5. Aplicar la misma rubrica a todos.
6. Crear el reporte siguiendo `skill/references/reporte-notion.md`.
7. Publicar el resultado con el MCP oficial de Notion.
8. Volver a leer la pagina publicada y entregar su enlace.

## Prompt sugerido

```text
Usa el skill de este repositorio. Compara todos los candidatos de la carpeta
candidates con las dos vacantes de la carpeta jobs. Clasifica cada persona
para el puesto A, puesto B, ambos o ninguno, prioriza a quien contactar y
publica el reporte en Notion.
```

## Reglas importantes

- La recomendacion sirve para revision humana; no toma la decision final de contratacion.
- Usar solo experiencia, habilidades, idiomas y condiciones laborales escritas.
- Se puede considerar disponibilidad para trabajar desde Latinoamerica.
- No usar nacionalidad, edad, genero, fotografia u otros datos personales sensibles.
- No inventar informacion ausente. Marcarla como `Por confirmar`.
- No publicar datos de contacto completos ni los PDFs en Notion.

