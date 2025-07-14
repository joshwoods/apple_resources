

- MapKit
-  MKOverlayLevel 

Enumeration

# MKOverlayLevel

Constants that indicate the position of overlays relative to other content.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 10.0+

``` source
enum MKOverlayLevel
```

## Topics

### Constants

case aboveRoads

Place the overlay above roadways but below map labels, shields, or point-of-interest icons.

case aboveLabels

Place the overlay above map labels, shields, or point-of-interest icons but below annotations and 3D projections of buildings.

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

### Accessing overlays

var overlays: [any MKOverlay]

The overlay objects associated with the map view.

func overlays(in: MKOverlayLevel) -> [any MKOverlay]

Returns overlay objects in the specified level of the map.

func renderer(for: any MKOverlay) -> MKOverlayRenderer?

Returns the renderer object for drawing the contents of the specified overlay object.

func view(for: any MKOverlay) -> MKOverlayView

Returns the view associated with the overlay object, if any.

Deprecated

