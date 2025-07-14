

- ProximityReader
- VASRequest
- VASRequest.Merchant
-  url 

Instance Property

# url

The URL to display to the customer if the matching loyalty or reward ID isn’t found.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
let url: URL?
```

## Mentioned in 

Accepting loyalty passes from Wallet

## Discussion

If the customer isn’t part of the merchant’s loyalty program, they can use the provided URL to get more information about that program.

## See Also

### Getting the merchant URL details

let shouldSendURLOnly: Bool

A Boolean value that indicates whether to send only the merchant URL to the customer’s device without requesting data.

Deprecated

