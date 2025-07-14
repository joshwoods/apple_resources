

- ProximityReader
- MobileNationalIDCardDataRequest
-  nationalIDCardData(region:retaining:notRetaining:) 

Type Method

# nationalIDCardData(region:retaining:notRetaining:)

A request which retrieves elements from the holder and returns the validated document elements.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
static func nationalIDCardData(
    region: Locale.Region,
    retaining retainedElements: [MobileNationalIDCardDataRequest.Element] = [],
    notRetaining nonRetainedElements: [MobileNationalIDCardDataRequest.Element] = []
) -> Self
```

Available when `Self` is `MobileNationalIDCardDataRequest`.

