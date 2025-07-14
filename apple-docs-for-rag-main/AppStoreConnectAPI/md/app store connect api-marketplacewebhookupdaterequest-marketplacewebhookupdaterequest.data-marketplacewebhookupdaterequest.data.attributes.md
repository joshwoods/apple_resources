

- App Store Connect API
- MarketplaceWebhookUpdateRequest
- MarketplaceWebhookUpdateRequest.Data
-  MarketplaceWebhookUpdateRequest.Data.Attributes 

Object

# MarketplaceWebhookUpdateRequest.Data.Attributes

Attributes that describe a marketplace webhook resource.

App Store Connect API 3.3+

``` source
object MarketplaceWebhookUpdateRequest.Data.Attributes
```

## Properties

`endpointUrl`

`uri`

`secret`

`string`

An arbitrary string. Alternative marketplaces use this secret string to verify the incoming requests from Apple about changes to apps. For more information about webhook-style validation, see Github’s Validating webhook deliveries.

For more information about implementing Hash-based Message Authentication Code (HMAC) security in your notifications webhook, see Processing alternative app marketplace notifications.

