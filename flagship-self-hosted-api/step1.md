

## 1. Configure Flagship Self-Hosted Decision API

Open the config file and fillout your Flagship Environment ID & API Key.
You can get them [Here](https://app.flagship.io/)

`config.yaml`{{open}}

## 2. Start Flagship Self-Hosted Decision API

`docker run -p 8080:8080 -v $(pwd)/config.yaml:/config.yaml -d flagshipio/self-hosted-api`{{execute}}

## 3. Test the Decision API

`curl -X POST -H 'Content-Type: application/json' -d '{"visitor_id":"vid","context": {}}' localhost:8080/v2/campaigns`{{execute}}

## 4. Open the Swagger UI for the API Reference

https://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katacoda.com/v2/swagger/index.html

