

- App Store Connect API
-  Delete a queue 

Web Service Endpoint

# Delete a queue

Delete a specific queue in a rule set.

App Store Connect API 3.1+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the queue.

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Creating, modifying, and deleting queues

Create a queue

Create a queue and add it to a rule set.

Modify a queue

Update the properties of a specific queue.

