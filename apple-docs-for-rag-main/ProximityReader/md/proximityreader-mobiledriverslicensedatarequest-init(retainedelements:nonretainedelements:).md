

- ProximityReader
- MobileDriversLicenseDataRequest
-  init(retainedElements:nonRetainedElements:) 

Initializer

# init(retainedElements:nonRetainedElements:)

Returns a mobile driver’s license data request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
init(
    retainedElements: [MobileDriversLicenseDataRequest.Element] = [],
    nonRetainedElements: [MobileDriversLicenseDataRequest.Element] = []
)
```

## See Also

### Creating a data request

var retainedElements: [MobileDriversLicenseDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileDriversLicenseDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than necessary to process the result in realtime.

struct Element

A type that represents an element you can request from a mobile driver’s license.

