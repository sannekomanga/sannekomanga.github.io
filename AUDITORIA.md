# AUDITORÍA DEL REPOSITORIO

**Fecha:** 2026-11-21 13:26 UTC  
**Auditor:** Auditor Automático v2.1  
**Modo:** Solo lectura — Repositorio completo  
**Estado:** COMPLETADA CON LIMITACIONES

## Resumen

La revisión local (gitleaks + semgrep + heurísticas) se ejecutó correctamente.  
El análisis de IA no pudo completarse: `Error code: 400 - {'type': 'error', 'error': {'type': 'invalid_request_error', 'message': 'Your credit balance is too low to access the Anthropic API. Please go to Plans & Billing to upgrade or purchase credits.'}, 'request_id': 'req_011ChG9brDC11rNK4sbnt3CH'}`

## Métricas

| Métrica | Valor |
|---------|-------|
| Archivos analizados | 15 |
| Archivos críticos | 4 |
| Bytes leídos | 126,850 |
| Hallazgos locales | 3 |
| Duración | 0.0s |
| Evento | schedule |

## Hallazgos preliminares (herramientas locales)

| ID | Severidad | Archivo | Hallazgo | Estado |
|---|---|---|---|---|
| AUD-001 | MEDIO | auditor/auditor.py | [heuristics] Posible referencia a service_role de Supabase  | PENDIENTE |
| AUD-002 | CRÍTICO | auditor/auditor.py | [heuristics] Posible clave de API de proveedor de pagos/LLM  | PENDIENTE |
| AUD-003 | CRÍTICO | auditor/auditor.py | [heuristics] Posible token de Slack/GitHub  | PENDIENTE |

## Recomendaciones

- Revisar manualmente los indicadores anteriores.
- Configurar `OPENAI_API_KEY` o `ANTHROPIC_API_KEY` en GitHub Actions Secrets.
- No colocar claves privadas ni tokens directamente en el repositorio.

## Regla del auditor

Este proceso **informa** sobre hallazgos y **no modifica** el código del proyecto (solo actualiza `AUDITORIA.md`).

## Historial

Las ejecuciones posteriores añadirán una entrada con fecha, resumen y hallazgos.

---

**Regla:** este auditor informa; no modifica archivos del proyecto salvo `AUDITORIA.md`.
### 2026-11-16 13:35 UTC
- Archivos: 15 | Hallazgos locales: 3 | Evento: schedule
### 2026-11-17 14:20 UTC
- Archivos: 15 | Hallazgos locales: 3 | Evento: schedule
### 2026-11-18 13:54 UTC
- Archivos: 15 | Hallazgos locales: 3 | Evento: schedule
### 2026-11-19 14:23 UTC
- Archivos: 15 | Hallazgos locales: 3 | Evento: schedule
### 2026-11-20 13:58 UTC
- Archivos: 15 | Hallazgos locales: 3 | Evento: schedule
### 2026-11-21 13:26 UTC
- Archivos: 15 | Hallazgos locales: 3 | Evento: schedule
