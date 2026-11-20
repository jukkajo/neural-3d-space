# Contributing

This project follows a lightweight branch-based workflow. Workflows should be updated to match current needs. Changes should be developed on short-lived branches and merged into `main` after verification. The purpose of this file is to support maintainability and consistent development practices.

## Branching Convention

Branches should contain one logical change and use:

```text
<type>/<short-description>
```

### Types

| Type       | Use                                  |
| ---------- | ------------------------------------ |
| `feat`     | New functionality                    |
| `fix`      | Defect correction                    |
| `refactor` | Behavior-preserving restructuring    |
| `test`     | Test-only changes                    |
| `docs`     | Documentation changes                |
| `build`    | Build, dependency, or Docker changes |
| `ci`       | Continuous-integration changes       |
| `chore`    | Repository maintenance               |

Examples:

```text
feat/people-directory-parser
feat/freebusy-parser
fix/interval-boundary-handling
docs/document-business-rules
build/minimize-docker-image
```

## Commit Convention

Use Conventional Commits:

```text
<type>(<scope>): <summary>
```

Examples:

```text
feat(scheduling): add people directory parser
fix(scheduling): handle adjacent busy intervals
test(scheduling): cover invalid freebusy periods
docs(adr): document in-memory reference data
build(docker): add production image
```

Common commit types:

```text
feat, fix, refactor, perf, test, docs, build, ci, chore, revert
```

Keep commit summaries concise and lowercased.

## Documentation

Significant architectural decisions should be recorded as Architecture Decision Records under `docs/adr/`.

Implementation and design details like domain models or complex concepts belong under `docs/design/` when they require explanation beyond the source code.
