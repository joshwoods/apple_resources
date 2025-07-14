

- Foundation
- Locale
- Locale.Region
-  subRegions 

Instance Property

# subRegions

An array of all the sub-regions of the region.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var subRegions: [Locale.Region] { get }
```

## Discussion

The following example looks up the sub-regions of region `021`, which represents North America.

```
let northAmericaRegion = Locale.Region("021")
let subRegions = northAmericaRegion.subRegions //BM, CA, GL, PM, US
```

The returned `subRegions` have the following identifiers:

| Identifier | Country                   |
|------------|---------------------------|
| BM         | Bermuda                   |
| CA         | Canada                    |
| GL         | Greenland                 |
| PM         | Saint Pierre and Miquelon |
| US         | United States             |

## See Also

### Examining region properties

var identifier: String

The BCP 47 identifier of the region.

var containingRegion: Locale.Region?

The region that contains this region, if any.

var continent: Locale.Region?

The continent that contains this region, if any.

var isISORegion: Bool

A Boolean value that indicates whether the region is an ISO-defined region.

