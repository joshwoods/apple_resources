

- ProximityReader
- VASRequest
-  init(vasMerchants:localizedVASType:) 

Initializer

# init(vasMerchants:localizedVASType:)

Creates a request to read loyalty card service information.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
init(
    vasMerchants: [VASRequest.Merchant] = [],
    localizedVASType: String = ""
)
```

## Parameters 

`vasMerchants`  

The merchants associated with the requested loyalty program.

`localizedVASType`  

The localized name of the loyalty program.

