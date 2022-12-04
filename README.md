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
### Start container

```yaml
# either flask run and bind 5000 on start
command: sh -c 'cd .. && flask run' # this doesn't work
ports:
    - '5000:5000'

# or sleep infinity and leave 5000 free, then flask run will ask vs code to forward port
command: sleep infinity # that's it
flask run # in terminal
# can use or not, either is fine
"forwardPorts": [5000],
```

