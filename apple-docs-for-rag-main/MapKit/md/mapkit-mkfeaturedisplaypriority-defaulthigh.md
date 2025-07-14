

- MapKit
- MKFeatureDisplayPriority
-  defaultHigh 

Type Property

# defaultHigh

A constant indicating that the item’s display priority is high.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let defaultHigh: MKFeatureDisplayPriority
```

## Discussion

An annotation view with this priority is removed from the map when its bounds collide with the bounds of another view with a higher priority. If the priorities of the two views are equal, the view furthest from the center of the map’s visible region is hidden first.

## See Also

### Priorities

static let required: MKFeatureDisplayPriority

A constant indicating that the item is required.

static let defaultLow: MKFeatureDisplayPriority

A constant indicating that the item’s display priority is low.

