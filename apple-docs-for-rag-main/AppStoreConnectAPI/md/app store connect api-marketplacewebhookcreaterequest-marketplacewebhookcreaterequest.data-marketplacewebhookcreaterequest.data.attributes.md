

- App Store Connect API
- MarketplaceWebhookCreateRequest
- MarketplaceWebhookCreateRequest.Data
-  MarketplaceWebhookCreateRequest.Data.Attributes 

Object

# MarketplaceWebhookCreateRequest.Data.Attributes

The attributes you set that describe the marketplace webhook used to create a new resource.

App Store Connect API 3.3+

``` source
object MarketplaceWebhookCreateRequest.Data.Attributes
```

## Properties

`endpointUrl`

`uri`

 (Required) 

`secret`

`string`

 (Required) 

An arbitrary string. Alternative marketplaces use this secret string to verify the incoming requests from Apple about changes to apps. For more information about webhook-style validation, see Github’s Validating webhook deliveries.

For more information about implementing Hash-based Message Authentication Code (HMAC) security in your notifications webhook, see Processing alternative app marketplace notifications.

