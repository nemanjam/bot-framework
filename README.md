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

### Start app

```bash
flask run
```

### New how to run in container

```bash
# migrate db
alembic -c migrations/alembic.ini -x db=dev upgrade head

# run flask on port 5000
flask run


```