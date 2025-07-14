

- ProximityReader
- VASRequest
- VASRequest.Merchant
-  id 

Instance Property

# id

A unique identifier for the merchant.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
let id: String
```

## Discussion

When reading a card, the system sends this identifier to the customer device, which uses the value to retrieve the matching loyalty or reward ID of the customer.

