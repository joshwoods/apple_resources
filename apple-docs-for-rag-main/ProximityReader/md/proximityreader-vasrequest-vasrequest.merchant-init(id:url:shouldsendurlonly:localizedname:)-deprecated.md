

- ProximityReader
- VASRequest
- VASRequest.Merchant
-  init(id:url:shouldSendURLOnly:localizedName:) Deprecated

Initializer

# init(id:url:shouldSendURLOnly:localizedName:)

Creates a new merchant object with the specified information.

iOS 15.4–16.4DeprecatediPadOS 15.4–16.4DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
init(
    id: String,
    url: URL? = nil,
    shouldSendURLOnly: Bool = false,
    localizedName: String? = nil
)
```

Deprecated

Not supported

## Parameters 

`id`  

The merchant’s unique identifier. Obtain this value from the merchant.

`url`  

The URL to display if the customer doesn’t belong to the merchant’s loyalty program.

`shouldSendURLOnly`  

A Boolean value that indicates whether to send the URL information to the customer’s device.

`localizedName`  

The name of the merchant, localized for the current device.

