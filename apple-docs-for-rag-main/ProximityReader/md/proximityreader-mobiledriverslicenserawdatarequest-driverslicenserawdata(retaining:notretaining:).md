

- ProximityReader
- MobileDriversLicenseRawDataRequest
-  driversLicenseRawData(retaining:notRetaining:) 

Type Method

# driversLicenseRawData(retaining:notRetaining:)

A request which retrieves mobile driver’s license elements from the holder and returns the raw response data for processing.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
static func driversLicenseRawData(
    retaining retainedElements: [MobileDriversLicenseRawDataRequest.Element],
    notRetaining nonRetainedElements: [MobileDriversLicenseRawDataRequest.Element]
) -> Self
```

Available when `Self` is `MobileDriversLicenseRawDataRequest`.

