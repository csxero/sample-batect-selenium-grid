# Sample project for selenium grid

## Run the grid

### Using docker compose

```bash
docker-compose up
```

or

### batect

```bash
./batect test-grid
```

## Then create a session using curl or postman

```bash
curl -fsS "http://localhost:7777/wd/hub/session" -XPOST --header "Accept: application/json" --header "Content-Type: application/json;charset=utf-8"--data "{'desiredCapabilities':{'browserName': 'chrome'}}"
```
