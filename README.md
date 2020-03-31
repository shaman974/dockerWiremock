# DOCKER ET wiremock

http://wiremock.org/

Exemple de lancement avec docker


docker run -d -p 8080:8080 -v /Users/vetranoromain/wiremock:/home/wiremock rodolpheche/wiremock -v /Users/vetranoromain/wiremock/extensions:/var/wiremock/extensions  --record-mappings --verbose --global-response-templating

verbose : affichage des requetes

global-response-templating : active les templates