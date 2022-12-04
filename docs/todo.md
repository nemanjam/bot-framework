
### Todo

- read flask_for_startups readme
- ask javascript python analogies, node_modules docker volumes, locations, venv
- how is 5000 exposed?

- add react, now bare js
- install dependencies in venv - in Dockerfile probably
- write db seed and start container properly, use .vscode/launch.json
- naming system services in docker-compose.yml
- update dependencies
- setup format on save, .vscode/settings.json

### docker-compose.yml separate folder - ask

```yaml
# flask run from another folder fails, doesn't load .flaskenv
command: sh -c 'cd .. && flask run'
```