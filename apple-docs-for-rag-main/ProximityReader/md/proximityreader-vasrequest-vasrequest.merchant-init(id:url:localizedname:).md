

- ProximityReader
- VASRequest
- VASRequest.Merchant
-  init(id:url:localizedName:) 

Initializer

# init(id:url:localizedName:)

Creates a new merchant object with the specified information.

iOS 16.4+iPadOS 16.4+Mac Catalyst 17.0+

``` source
init(
    id: String,
    url: URL? = nil,
    localizedName: String? = nil
)
```

## Parameters 

`id`  

The merchant’s unique identifier. Obtain this value from the merchant.

`url`  

The URL to display if the customer doesn’t belong to the merchant’s loyalty program.

`localizedName`  

The name of the merchant, localized for the current device.

