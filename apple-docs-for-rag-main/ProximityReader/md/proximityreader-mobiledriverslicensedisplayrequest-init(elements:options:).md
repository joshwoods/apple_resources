

- ProximityReader
- MobileDriversLicenseDisplayRequest
-  init(elements:options:) 

Initializer

# init(elements:options:)

Creates a new mobile driver’s license display request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
init(
    elements: [MobileDriversLicenseDisplayRequest.Element] = [],
    options: MobileDriversLicenseDisplayRequest.Options = .init()
)
```

## See Also

### Creating a display request

var elements: [MobileDriversLicenseDisplayRequest.Element]

The document elements you’re requesting.

struct Element

A type that represents an element you can request from a mobile driver’s license.

