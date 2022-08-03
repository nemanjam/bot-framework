# flask bot

### Forked from:

- https://github.com/nuvic/flask_for_startups

### Run migration with

```bash
PYTHONPATH=. alembic -c migrations/alembic.ini -x db=dev upgrade head
```

### Lint and format

- lint: `flake8`, format: `black`

- double definitions:

```ts
// extensions, settings (format, lint)
// .devcontainer/devcontainer.json

// .vscode/extensions.json
// .vscode/settings.json
```