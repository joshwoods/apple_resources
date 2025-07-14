

- ProximityReader
- MobileDriversLicenseDataRequest
-  nonRetainedElements 

Instance Property

# nonRetainedElements

The document elements you’re requesting and intend to retain no longer than necessary to process the result in realtime.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var nonRetainedElements: [MobileDriversLicenseDataRequest.Element]
```

## See Also

### Creating a data request

init(retainedElements: [MobileDriversLicenseDataRequest.Element], nonRetainedElements: [MobileDriversLicenseDataRequest.Element])

Returns a mobile driver’s license data request.

var retainedElements: [MobileDriversLicenseDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

struct Element

A type that represents an element you can request from a mobile driver’s license.

