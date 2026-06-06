# Conectar Notion MCP

Usar el servidor oficial:

```text
https://mcp.notion.com/mcp
```

La conexion abre Notion para que cada persona autorice su propio espacio de trabajo. No compartir claves ni contrasenas.

## Codex

### Opcion por terminal

```bash
codex mcp add notion --url https://mcp.notion.com/mcp
codex mcp login notion
codex mcp list
```

Completar la autorizacion de Notion en el navegador.

### Opcion por archivo

Agregar esto a `~/.codex/config.toml` para usarlo en todos los proyectos:

```toml
[mcp_servers.notion]
url = "https://mcp.notion.com/mcp"
```

Despues ejecutar:

```bash
codex mcp login notion
```

Para configurarlo solo en este repositorio, usar `.codex/config.toml` con el mismo contenido.

## Cowork

1. Abrir Cowork o Claude.
2. Entrar a `Settings`.
3. Abrir `Connectors`.
4. Elegir `Add connector` o `Add custom connector`.
5. Escribir `Notion` como nombre.
6. Pegar `https://mcp.notion.com/mcp` como direccion.
7. Pulsar `Connect`.
8. Autorizar el espacio de trabajo de Notion.
9. Activar el conector en la conversacion donde se ejecutara el skill.

En cuentas Team o Enterprise, un administrador puede necesitar agregar primero el conector para la organizacion.

## OpenCode

Crear `opencode.json` en la raiz del proyecto:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "mcp": {
    "notion": {
      "type": "remote",
      "url": "https://mcp.notion.com/mcp",
      "enabled": true
    }
  },
  "instructions": [
    "agent.md"
  ]
}
```

Abrir OpenCode en la carpeta del repositorio. Cuando Notion se use por primera vez, completar la autorizacion solicitada.

Para configurarlo en todos los proyectos, guardar esa configuracion en:

```text
~/.config/opencode/opencode.json
```

## Comprobacion

Pedir al agente:

```text
Crea una pagina privada en Notion llamada Prueba MCP y devuelve el enlace.
```

Si puede crear la pagina y devolver el enlace, la conexion funciona.

## Ejecutar con vacantes nuevas

1. Crear una carpeta `candidates` con los perfiles PDF.
2. Crear una carpeta `jobs` con exactamente dos vacantes PDF.
3. Abrir el repositorio en Codex, Cowork u OpenCode.
4. Usar este mensaje:

```text
Lee agent.md y ejecuta el skill con los PDFs de candidates y jobs.
Publica el reporte en una pagina privada de Notion y devuelve el enlace.
```

5. Revisar el reporte antes de contactar o descartar candidatos.

## Problemas comunes

- Si Notion no aparece, reiniciar la aplicacion despues de guardar la configuracion.
- Si pide acceso otra vez, desconectar y repetir la autorizacion.
- Si no puede publicar, comprobar que la cuenta tiene permiso para crear paginas.
- Verificar que la direccion sea exactamente `https://mcp.notion.com/mcp`.

## Documentacion oficial

- Notion MCP: https://developers.notion.com/docs/get-started-with-mcp
- Seguridad de Notion MCP: https://developers.notion.com/docs/mcp-security-best-practices
- Codex MCP: https://platform.openai.com/docs/docs-mcp
- Cowork y conectores remotos: https://support.anthropic.com/en/articles/11175166-getting-started-with-custom-integrations-using-remote-mcp
- OpenCode MCP: https://opencode.ai/docs/mcp-servers/

