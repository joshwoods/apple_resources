

- App Store Connect API
-  Read marketplace webhook information 

Web Service Endpoint

# Read marketplace webhook information

Get the endpoint URL for alternative distribution package notifications.

App Store Connect API 3.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks
```

## Query Parameters

`fields[marketplaceWebhooks]`

`[string]`

Value: `endpointUrl`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

MarketplaceWebhooksResponse

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

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks
```

```
{
  "data": [
    {
      "type": "marketplaceWebhooks",
      "id": "c74970b8-6be0-40fa-8f51-8e1532005635",
      "attributes": {
        "endpointUrl": "https://example.com/api/ingest/notifications"
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks/c74970b8-6be0-40fa-8f51-8e1532005635"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/marketplaceWebhooks"
  },
  "meta": {
    "paging": {
      "total": 1,
      "limit": 50
    }
  }
}

```

## See Also

### Managing Webhook Endpoint URLs

Add a marketplace webhook configuration

Add a new endpoint URL and secret for alternative distribution package notifications.

Modify a marketplace webhook configuration

Update the endpoint URL and secret for alternative distribution package notifications.

Delete a marketplace webhook configuration

Delete a specific marketplace notifcation endpoint URL.

