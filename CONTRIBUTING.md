# Cómo contribuir

Guía de trabajo para los repositorios de JAPAMI · Desarrollo de Software.

## 🌿 Ramas

| Rama | Uso |
|------|-----|
| `main` | Código en producción |
| `develop` | Integración y pruebas en QA |
| `feature/descripcion-corta` | Nueva funcionalidad |
| `fix/descripcion-corta` | Corrección de errores |
| `hotfix/descripcion-corta` | Corrección urgente en producción |

- Las ramas salen de `develop`, excepto `hotfix/`, que sale de `main`.
- Nombres en minúsculas, separados por guiones y sin acentos.

## ✍️ Commits

Usamos [Conventional Commits](https://www.conventionalcommits.org/es/):

```
<tipo>: <descripción en presente y en minúsculas>
```

| Tipo | Cuándo usarlo |
|------|---------------|
| `feat` | Nueva funcionalidad |
| `fix` | Corrección de un error |
| `refactor` | Cambio de código sin cambiar comportamiento |
| `docs` | Solo documentación |
| `test` | Agregar o corregir pruebas |
| `chore` | Mantenimiento, dependencias, configuración |

Ejemplos:
```
feat: agrega consulta de adeudos por cuenta
fix: corrige validación de fecha en formulario
chore: actualiza dependencias
```

## 🔀 Pull requests

1. Abre el PR hacia `develop` (o hacia `main` si es `hotfix/`).
2. Describe **qué cambia**, **por qué** y **cómo probarlo**.
3. Mantén los PRs pequeños; es mejor revisar varios chicos que uno enorme.
4. Todos los checks automáticos deben pasar.

**Reglas de revisión**
- Nadie hace merge de su propio PR.
- Se requiere al menos una aprobación.
- No se aprueba un PR con hallazgos críticos de seguridad abiertos.

## 🔒 Seguridad

- Nunca subas credenciales, cadenas de conexión, tokens ni llaves al repositorio.
- Usa variables de entorno o *secrets* de GitHub Actions.
- Si un secreto se sube por error, avisa de inmediato: debe rotarse, no basta con borrar el commit.

## 💬 Dudas

Contacta a [desarrollo@japami.gob.mx](mailto:desarrollo@japami.gob.mx).
