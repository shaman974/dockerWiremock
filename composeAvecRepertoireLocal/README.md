# Wiremok en docker compose avec repertoire externe pour les stub

## Lancement

```
docker-compose up -d
```

volume externe mappé : ../composeAvecStubDansImage

## test

```
curl http://localhost:8080/__admin/
```

```
curl http://localhost:8080/coefficient?courtier=ee06A&option=RIDER
```