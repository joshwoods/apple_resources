

- App Store Connect API
-  Read Actor Information 

Web Service Endpoint

# Read Actor Information

Get information about a specific actor.

App Store Connect API 2.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/actors/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the Read review submission information response with the include ReviewSubmission.Relationships.SubmittedByActor.

## Query Parameters

`fields[actors]`

`[string]`

Possible Values: `actorType, userFirstName, userLastName, userEmail, apiKeyId`

## Response Codes

` 200 ``OK`

ActorResponse

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/actors/USER:2cd2a1ef-cb74-411c-a078-0ebe119ade73
```

```
{
  “data” : {
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
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/actors/USER%3A2cd2a1ef-cb74-411c-a078-0ebe119ade73”
  }
}
```

## See Also

### Reading actor information

List All Actors

Get a list of actors.

