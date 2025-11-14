# Curso 2025 - Equipo 1

Repositorio del equipo para prácticas de Git y flujo de trabajo

\## Flujo de trabajo para el equipo

\*\* Flujo de trabajo elegido: Git Flow \*\*

* ¿Por qué elegimos este flujo de trabajo?

Básicamente es más simple y directo.

main es nuestra rama principal y la protegida, trabajamos en una rama y hcaemos commits

y pushes. Se abre un PR para revisión y después de ella se hacae un merge.

Consideramos que es un flujo de trabajo más lineal y rápido.



### 4.1 Nombres de ramas (copiar/pegar al README)

-   **Features nuevas:** `feature/<tema-kebab-case>`
    
    -   Ej: `feature/api-health-endpoint`, `feature/ui-login-form`
        
-   **Bugs urgentes en producción:** `hotfix/<bug-descriptivo>`
    
    -   Ej: `hotfix/fix-nullref-on-auth`
        
-   **Versiones de release (solo Git Flow):** `release/<version>`
    
    -   Ej: `release/1.2.0`
        

> Reglas rápidas: minúsculas, sin espacios, usa `-` para separar palabras.

### 4.2 Convención de commits (Conventional Commits + ejemplos)

**Formato:**

```
<type>(<scope>): <mensaje en imperativo>

```

**Tipos comunes:**

-   `feat` (nueva funcionalidad)
    
-   `fix` (arreglo de bug)
    
-   `docs` (documentación)
    
-   `chore` (mantenimiento, ajustes no funcionales)
    
-   `refactor` (cambia estructura sin cambiar comportamiento)
    
-   `test` (añade o ajusta pruebas)
    
-   `build` (cambios en build, dependencias)
    
-   `ci` (cambios en pipelines)
    

**Scope** (opcional): `api`, `db`, `ui`, `infra`, `auth`, etc.

**Ejemplos buenos:**

```text
feat(api): añade endpoint /health
fix(auth): corrige validación de token expirado
docs(readme): agrega diagrama de flujo git
refactor(db): separa repositorio de consultas
ci(workflow): agrega job de build en PRs
chore(repo): inicializa .gitignore y license

```

**Ejemplos a evitar:**

```text
update files
fix stuff
final version

```
