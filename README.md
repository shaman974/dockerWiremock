# DOCKER ET wiremock

## Liens utiles

http://wiremock.org/

https://hub.docker.com/r/rodolpheche/wiremock/

## Exemple

Exemple de lancement avec docker avec un repertoire :
- pour les stub : /home/wiremock
- pour les extensions : /var/wiremock/extensions

```
mkdir wiremock
mkdir extension

docker run -d -p 8080:8080 -v $PWD/wiremock:/home/wiremock rodolpheche/wiremock -v $PWD/wiremock/extensions:/var/wiremock/extensions  --record-mappings --verbose --global-response-templating
```

## Paramètres utiles

verbose : affichage des requetes

global-response-templating : active les templates
