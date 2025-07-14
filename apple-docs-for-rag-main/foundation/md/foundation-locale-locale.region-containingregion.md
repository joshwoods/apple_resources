

- Foundation
- Locale
- Locale.Region
-  containingRegion 

Instance Property

# containingRegion

The region that contains this region, if any.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var containingRegion: Locale.Region? { get }
```

## Discussion

The following example shows how to look up the containing region for the `US` region.

```
let usRegion = Locale.Region("US")
let containingRegion = usRegion.containingRegion //Identifier "021": Northern America

```

## See Also

### Examining region properties

var identifier: String

The BCP 47 identifier of the region.

var continent: Locale.Region?

The continent that contains this region, if any.

var isISORegion: Bool

A Boolean value that indicates whether the region is an ISO-defined region.

var subRegions: [Locale.Region]

An array of all the sub-regions of the region.

