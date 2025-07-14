

- MapKit
-  MKLookAroundBadgePosition 

Enumeration

# MKLookAroundBadgePosition

Constants that control the position of badges on LookAround views.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
enum MKLookAroundBadgePosition
```

## Topics

### Badge positions

case bottomTrailing

The value that indicates the bottom-right badge position.

case topLeading

The value that indicates the top-left badge position.

case topTrailing

The value that indicates the top-right badge position.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing the LookAround display

var isNavigationEnabled: Bool

A Boolean value that indicates whether the map’s navigation controls are visible.

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter used to determine the points of interest shown on the map.

var showsRoadLabels: Bool

A Boolean value that indicates whether the map display road labels.

var badgePosition: MKLookAroundBadgePosition

A value that indicates the badge’s position on the LookAround view.

