

- ProximityReader
- MobileNationalIDCardRawDataRequest
-  nationalIDCardRawData(region:retaining:notRetaining:) 

Type Method

# nationalIDCardRawData(region:retaining:notRetaining:)

A request which retrieves mobile national ID card elements from the holder and returns the raw response data for processing.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
static func nationalIDCardRawData(
    region: Locale.Region,
    retaining retainedElements: [MobileNationalIDCardRawDataRequest.Element] = [],
    notRetaining nonRetainedElements: [MobileNationalIDCardRawDataRequest.Element] = []
) -> Self
```

Available when `Self` is `MobileNationalIDCardRawDataRequest`.

