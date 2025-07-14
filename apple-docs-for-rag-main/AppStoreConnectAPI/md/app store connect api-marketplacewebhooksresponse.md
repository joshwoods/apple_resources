

- App Store Connect API
-  MarketplaceWebhooksResponse 

Object

# MarketplaceWebhooksResponse

A response that contains a list of a marketplace webhook resources.

App Store Connect API 3.3+

``` source
object MarketplaceWebhooksResponse
```

## Properties

`data`

`[`MarketplaceWebhook`]`

 (Required) 

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## Discussion

Use this object with Read marketplace webhook information.

## See Also

### Objects

object MarketplaceWebhook

The data structure that represents a marketplace webhook resource.

object MarketplaceWebhookCreateRequest

The request body you use to create a marketplace webhook url.

object MarketplaceWebhookResponse

A response that contains a single marketplace webhook resource.

object MarketplaceWebhookUpdateRequest

The request body you use to update a marketplace webhook url.

