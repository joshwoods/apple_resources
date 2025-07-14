

- App Store Connect API
-  MarketplaceWebhook 

Object

# MarketplaceWebhook

The data structure that represents a marketplace webhook resource.

App Store Connect API 3.3+

``` source
object MarketplaceWebhook
```

## Properties

`attributes`

MarketplaceWebhook.Attributes

`id`

`string`

 (Required) 

`links`

ResourceLinks

`type`

`string`

 (Required) 

Value: `marketplaceWebhooks`

## Topics

### Objects

object MarketplaceWebhook.Attributes

The attribute that describes the url where you will recieve notifications.

## See Also

### Objects

object MarketplaceWebhookCreateRequest

The request body you use to create a marketplace webhook url.

object MarketplaceWebhookResponse

A response that contains a single marketplace webhook resource.

object MarketplaceWebhooksResponse

A response that contains a list of a marketplace webhook resources.

object MarketplaceWebhookUpdateRequest

The request body you use to update a marketplace webhook url.

