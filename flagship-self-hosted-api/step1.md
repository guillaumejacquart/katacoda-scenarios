

## Configure Flagship Self-Hosted API

Open the config file and fillout your Flagship Environment ID & API Key.
You can get them [Here](https://app.flagship.io/)

`config.yaml`{{open}}

## Start Flagship Self-Hosted API

`docker run -p 8080:8080 -v $(pwd)/config.yaml:/config.yaml -d flagshipio/self-hosted-api`{{execute}}

## Test

`curl -X POST -H 'Content-Type: application/json' -d '{"visitor_id":"vid","context": {}}' localhost:8080/v2/campaigns`{{execute}}

## Open the Swagger UI for the API Reference

https://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katacoda.com/v2/swagger/index.html

## Markdown

<pre>https://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katacoda.com/v2/swagger/index.html</pre>

## Learn More

[Displaying Tabs](https://katacoda.com/scenario-examples/scenarios/dashboard-tabs) and [embedding iFrames](https://katacoda.com/scenario-examples/scenarios/dashboard-tabs-iframe)