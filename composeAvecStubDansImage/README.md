# Wiremok en docker compose avec build de l'image et des stub

## build de l'image

```
docker build . -t perso-wiremock
```

## Lancement

```
docker-compose up -d
```

## test

```
curl http://localhost:8080/__admin/
```

```
curl http://localhost:8080/coefficient?courtier=ee06A&option=RIDER
```