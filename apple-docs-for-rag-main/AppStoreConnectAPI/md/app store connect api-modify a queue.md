

- App Store Connect API
-  Modify a queue 

Web Service Endpoint

# Modify a queue

Update the properties of a specific queue.

App Store Connect API 3.1+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the queue.

## HTTP Body

GameCenterMatchmakingQueueUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

GameCenterMatchmakingQueueResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Creating, modifying, and deleting queues

Create a queue

Create a queue and add it to a rule set.

Delete a queue

Delete a specific queue in a rule set.

