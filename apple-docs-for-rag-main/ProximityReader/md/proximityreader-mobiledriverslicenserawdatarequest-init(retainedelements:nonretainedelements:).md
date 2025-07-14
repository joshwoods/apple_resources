

- ProximityReader
- MobileDriversLicenseRawDataRequest
-  init(retainedElements:nonRetainedElements:) 

Initializer

# init(retainedElements:nonRetainedElements:)

Returns a mobile driver’s license raw data request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
init(
    retainedElements: [MobileDriversLicenseRawDataRequest.Element] = [],
    nonRetainedElements: [MobileDriversLicenseRawDataRequest.Element] = []
)
```

## See Also

### Creating a raw data request

var retainedElements: [MobileDriversLicenseRawDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileDriversLicenseRawDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than is necessary to process the result in realtime.

struct Element

A type representing an element that you can request from a mobile driver’s license.

