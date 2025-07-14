

- Foundation
- Locale
- Locale.Region
-  isISORegion 

Instance Property

# isISORegion

A Boolean value that indicates whether the region is an ISO-defined region.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var isISORegion: Bool { get }
```

## See Also

### Examining region properties

var identifier: String

The BCP 47 identifier of the region.

var containingRegion: Locale.Region?

The region that contains this region, if any.

var continent: Locale.Region?

The continent that contains this region, if any.

var subRegions: [Locale.Region]

An array of all the sub-regions of the region.

