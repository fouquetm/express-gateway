Tutorial de base : https://dev.to/naseef012/create-a-microservices-app-with-dockerized-express-api-gateway-1kf9

Tyk.io step by step tutorial : https://medium.com/geekculture/get-started-with-tyk-api-gateway-aae127186e1b

### json body to create bearer token:
'''
{
  "access_rights": {
    "1": {
      "api_name": "movie",
      "api_id": "1",
      "versions": ["Default"],
      "allowed_urls": null
    }
  },
  "org_id": "1"
}
'''

POST http://localhost:8080/tyk/keys
With header x-tyk-authorization key12345