

- ProximityReader
- MobileDocumentRequest
-  driversLicenseData(retaining:notRetaining:) 

Type Method

# driversLicenseData(retaining:notRetaining:)

A request which retrieves elements from the holder and returns the validated document elements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
static func driversLicenseData(
    retaining retainedElements: [MobileDriversLicenseDataRequest.Element],
    notRetaining nonRetainedElements: [MobileDriversLicenseDataRequest.Element]
) -> Self
```

Available when `Self` is `MobileDriversLicenseDataRequest`.

## See Also

### Mobile driver’s license data request

struct MobileDriversLicenseDataRequest

A mobile driver’s license request that retrieves elements from the holder and returns the validated document elements.

