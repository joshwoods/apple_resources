

- App Store Connect API
-  Create a queue 

Web Service Endpoint

# Create a queue

Create a queue and add it to a rule set.

App Store Connect API 3.1+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues
```

## HTTP Body

GameCenterMatchmakingQueueCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterMatchmakingQueueResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues
{
    “data”: {
        “type”: “gameCenterMatchmakingQueues”,
        “attributes”: {
            “referenceName”: “com.example.mygame.GameSettingsQueue”
        },
        “relationships”: {
            “ruleSet”: {
                “data”: {
                    “type”: “gameCenterMatchmakingRuleSets”,
                    “id”: “7353266e-8c6f-4cbe-8f0f-5108332a1146”
                }
            }
        }
    }
}
```

```
{
    “data”: {
        “type”: “gameCenterMatchmakingQueues”,
        “id”: “aa1c1e6b-f8a9-4bad-b969-860dfd1485c5”,
        “attributes”: {
            “referenceName”: “com.example.mygame.GameSettingsQueue”
        },
        “links”: {
            “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/aa1c1e6b-f8a9-4bad-b969-860dfd1485c5”
        }
    },
    “links”: {
        “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues”
    }
}
```

## See Also

### Creating, modifying, and deleting queues

Modify a queue

Update the properties of a specific queue.

Delete a queue

Delete a specific queue in a rule set.

