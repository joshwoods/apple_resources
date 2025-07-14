

- App Store Connect API
-  Delete a marketplace webhook configuration 

Web Service Endpoint

# Delete a marketplace webhook configuration

Delete a specific marketplace notifcation endpoint URL.

App Store Connect API 3.3+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `marketplaceWebhooks` resource ID from the Read marketplace webhook information response.

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

## Discussion

### Example Request and Response

- Request
- Response

```
DELETE https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks/c74970b8-6be0-40fa-8f51-8e1532005635
```

```
204
```

## See Also

### Managing Webhook Endpoint URLs

Read marketplace webhook information

Get the endpoint URL for alternative distribution package notifications.

Add a marketplace webhook configuration

Add a new endpoint URL and secret for alternative distribution package notifications.

Modify a marketplace webhook configuration

Update the endpoint URL and secret for alternative distribution package notifications.

