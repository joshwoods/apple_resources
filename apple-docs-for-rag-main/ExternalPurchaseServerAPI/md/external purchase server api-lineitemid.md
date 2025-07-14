

- External Purchase Server API
-  lineItemId 

Type

# lineItemId

A unique identifier for the line item, that you determine.

External Purchase Server API 1.0.0+

``` source
string lineItemId
```

## Mentioned in 

Reporting corrections

## Discussion

Maximum length: 128

The lineItemId string must be unique for each app. Using UUIDs is recommended. All line item objects have a lineItemId, including:

- OneTimeBuyLineItem

- RefundLineItem

- SubscriptionBuyLineItem

