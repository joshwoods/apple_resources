

- External Purchase Server API
-  productType 

Type

# productType

The type of product in the transaction, whether it’s a one-time buy, or a subscription.

External Purchase Server API 1.0.0+

``` source
string productType
```

## Possible Values 

`ONE_TIME_BUY`  

`SUBSCRIPTION`  

## Discussion

Allowed values: `ONE_TIME_BUY`, `SUBSCRIPTION`

Use `ONE_TIME_BUY` for in-app products that customers purchase once. Use `SUBSCRIPTION` for in-app products that have periodic renewals.

## See Also

### Providing product info

type productIdentifier

A string that identifies the product.

type quantity

The quantity of the product the customer purchased in a single transaction.

