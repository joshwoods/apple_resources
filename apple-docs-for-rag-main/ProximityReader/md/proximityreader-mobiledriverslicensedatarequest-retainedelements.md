

- ProximityReader
- MobileDriversLicenseDataRequest
-  retainedElements 

Instance Property

# retainedElements

The document elements you’re requesting and intend to retain for an indefinite period of time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var retainedElements: [MobileDriversLicenseDataRequest.Element]
```

## See Also

### Creating a data request

init(retainedElements: [MobileDriversLicenseDataRequest.Element], nonRetainedElements: [MobileDriversLicenseDataRequest.Element])

Returns a mobile driver’s license data request.

var nonRetainedElements: [MobileDriversLicenseDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than necessary to process the result in realtime.

struct Element

A type that represents an element you can request from a mobile driver’s license.

