

- App Store Connect API
-  List All Actors 

Web Service Endpoint

# List All Actors

Get a list of actors.

App Store Connect API 2.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/actors
```

## Query Parameters

`fields[actors]`

`[string]`

Possible Values: `actorType, userFirstName, userLastName, userEmail, apiKeyId`

`filter[id]`

`[string]`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the Read review submission information response with the include ReviewSubmission.Relationships.SubmittedByActor.

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

ActorsResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

## Discussion

This endpoint supports multiple id’s in the filter paramenter.

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/actors?filter%5Bid%5D=USER%3A2cd2a1ef-cb74-411c-a078-0ebe119ade73,USER%3A83f7ddc0-64d6-4e4f-a5d9-51d74a8009a3
```

```
{  “data” : [ {
    “type” : “actors”,
    “id” : “USER:83f7ddc0-64d6-4e4f-a5d9-51d74a8009a3”,
    “attributes” : {
      “actorType” : “USER”,
      “userFirstName” : “Maria”,
      “userLastName” : “Ruiz”,
      “userEmail” : “mruiz2@icloud.com”,
      “apiKeyId” : null
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/actors/USER%3A83f7ddc0-64d6-4e4f-a5d9-51d74a8009a3”
    }
  }, {
    “type” : “actors”,
    “id” : “USER:2cd2a1ef-cb74-411c-a078-0ebe119ade73”,
    “attributes” : {
      “actorType” : “USER”,
      “userFirstName” : “Bill”,
      “userLastName” : “James”,
      “userEmail” : “billjames2@icloud.com”,
      “apiKeyId” : null
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/actors/USER%3A2cd2a1ef-cb74-411c-a078-0ebe119ade73”
    }
  } ],
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/actors?filter%5Bid%5D=USER%3A2cd2a1ef-cb74-411c-a078-0ebe119ade73%2CUSER%3A83f7ddc0-64d6-4e4f-a5d9-51d74a8009a3”
  },
  “meta” : {
    “paging” : {
      “total” : 2,
      “limit” : 50
    }
  }
}

```

## See Also

### Reading actor information

Read Actor Information

Get information about a specific actor.

