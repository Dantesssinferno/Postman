```
Google Maps Add API (POST):
Add new place into Server

Base URL: https://rahulshettyacademy.com​ 
Resource: /maps/api/place/add/json
POST:
Query Parameters: key =qaclick123
Http Method: POST
Sample Body:
{
  "location": {
    "lat": -38.383494,
    "lng": 33.427362
  },
  "accuracy": 50,
  "name": "Frontline house",
  "phone_number": "(+91) 983 893 3937",
  "address": "29, side layout, cohen 09",
  "types": [
    "shoe park",
    "shop"
  ],
  "website": "http://google.com",
  "language": "French-IN"
}
Sample Response
{
    "status": "OK",
    "place_id": "5152b42a727f7904d5895c3fbaeb2dba",
    "scope": "APP",
    "reference": "7dcb62845bf503418b5e223c050d636c7dcb62845bf503418b5e223c050d636c",
    "id": "7dcb62845bf503418b5e223c050d636c"
}
GET:
https://rahulshettyacademy.com/maps/api/place/get/json?key=qaclick123&place_id=ed0c29bfef8f9ca2a3dc5ccfabfd5825
Base URL: https://rahulshettyacademy.com​ 
Resource: /maps/api/place/get/json
Query Parameters: key,  place_id //(place_id  value comes from Add place response)
Http request: GET
Query Parameters: key =qaclick123
Sample Response for the Provided Place_ID
Sample Response
{
    "location": {
        "latitude": "-38.383494",
        "longitude": "33.427362"
    },
    "accuracy": "50",
    "name": "Frontline house",
    "phone_number": "(+91) 983 893 3937",
    "address": "29, side layout, cohen 09",
    "types": "shoe park,shop",
    "website": "http://google.com",
    "language": "French-IN"
}

PUT:
Base URL: https://rahulshettyacademy.com​ 
Resource: /maps/api/place/update/json
Query Parameters: key =qaclick123
Http request: PUT
Sample Response
{
  "place_id":"5152b42a727f7904d5895c3fbaeb2dba",
  "address":"69 Krechatik UA Ukraine",
  "key":"qaclick123"
}

DELETE:
Base URL: https://rahulshettyacademy.com​ 
Resource: /maps/api/place/delete/json
Query Parameters: key =qaclick123
Http Method: DELETE
Sample Body:
{
  "place_id":"5152b42a727f7904d5895c3fbaeb2dba"
}

Sample Response
{
    “status”: ”OK”
}
```
