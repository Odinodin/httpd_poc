# HTTPD PoC
Testing Apache HTTPD config with Docker

## Start
`docker compose up --build`

## Stop
`docker compose down`

## Testing CORS
Requests from origin mydomain.com and otherdomain.no will get CORS headers

`curl -i -X OPTIONS -H "Origin: http://mydomain.com" http://localhost:8080/with-cors`