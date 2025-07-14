

- App Store Connect API
-  Add a marketplace webhook configuration 

Web Service Endpoint

# Add a marketplace webhook configuration

Add a new endpoint URL and secret for alternative distribution package notifications.

App Store Connect API 3.3+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks
```

## HTTP Body

MarketplaceWebhookCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

MarketplaceWebhookResponse

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

## Mentioned in 

Configuring alternative marketplaces and alternative marketplace apps

Creating alternative distribution packages

App Store Connect API 3.3 release notes

## Discussion

Each developer account has a single marketplace webhooks `endpointUrl`, so if you operate mutliple marketplaces all notifications come to a single endpoint. The notification payload contains the `marketplaceAppId.`

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks
{
  "data": {
    "type": "marketplaceWebhooks",
    "attributes": {
      "endpointUrl": "https://example.com/api/ingest/notifications",
      "secret": "mysecretstring"
    }
  }
}
```

```
{
  “data”: [
    {
      “type”: “marketplaceWebhooks”,
      “id”: “c74970b8-6be0-40fa-8f51-8e1532005635”,
      “attributes”: {
        “endpointUrl”: “https://example.com/api/ingest/notifications”
      },
      “links”: {
        “self”: “https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks/c74970b8-6be0-40fa-8f51-8e1532005635”
      }
    }
  ],
  “links”: {
    “self”: “https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks”
  },
  “meta”: {
    “paging”: {
      “total”: 1,
      “limit”: 50
    }
  }
}
```

## See Also

### Managing Webhook Endpoint URLs

Read marketplace webhook information

Get the endpoint URL for alternative distribution package notifications.

Modify a marketplace webhook configuration

Update the endpoint URL and secret for alternative distribution package notifications.

Delete a marketplace webhook configuration

Delete a specific marketplace notifcation endpoint URL.

