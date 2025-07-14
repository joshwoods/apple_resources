

- ProximityReader
- MobileDocumentRequest
-  nationalIDCard(region:\_:options:) 

Type Method

# nationalIDCard(region:\_:options:)

A request that displays national ID card elements onscreen.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
static func nationalIDCard(
    region: Locale.Region,
    _ elements: [MobileNationalIDCardDisplayRequest.Element],
    options: MobileNationalIDCardDisplayRequest.Options = .init()
) -> Self
```

Available when `Self` is `MobileNationalIDCardDisplayRequest`.

## See Also

### National ID card display request

struct MobileNationalIDCardDisplayRequest

A mobile national ID card request that retrieves elements from the holder and displays the results onscreen for visual inspection.

