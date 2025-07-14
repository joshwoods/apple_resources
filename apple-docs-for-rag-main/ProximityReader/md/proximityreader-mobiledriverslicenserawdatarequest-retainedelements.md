

- ProximityReader
- MobileDriversLicenseRawDataRequest
-  retainedElements 

Instance Property

# retainedElements

The document elements you’re requesting and intend to retain for an indefinite period of time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var retainedElements: [MobileDriversLicenseRawDataRequest.Element]
```

## See Also

### Creating a raw data request

init(retainedElements: [MobileDriversLicenseRawDataRequest.Element], nonRetainedElements: [MobileDriversLicenseRawDataRequest.Element])

Returns a mobile driver’s license raw data request.

var nonRetainedElements: [MobileDriversLicenseRawDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than is necessary to process the result in realtime.

struct Element

A type representing an element that you can request from a mobile driver’s license.

