

- Foundation
- Locale
- Locale.Region
-  continent 

Instance Property

# continent

The continent that contains this region, if any.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var continent: Locale.Region? { get }
```

## Discussion

This value can be `nil` when the system can’t determine the appropriate continent, such as when the region isn’t an ISO region.

## See Also

### Examining region properties

var identifier: String

The BCP 47 identifier of the region.

var containingRegion: Locale.Region?

The region that contains this region, if any.

var isISORegion: Bool

A Boolean value that indicates whether the region is an ISO-defined region.

var subRegions: [Locale.Region]

An array of all the sub-regions of the region.

