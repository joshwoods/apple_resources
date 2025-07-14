

- MapKit
-  MKMapType Deprecated

Enumeration

# MKMapType

The type of map to display.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
enum MKMapType
```

Deprecated

Use the map view’s preferredConfiguration property with one of the MKMapConfiguration subclasses to select a specific map style instead.

## Topics

### Constants

case standard

A street map that shows the position of all roads and some road names.

case satellite

Satellite imagery of the area.

case hybrid

A satellite image of the area with road and road name information layered on top.

case satelliteFlyover

A satellite image of the area with flyover data where available.

case hybridFlyover

A hybrid satellite image with flyover data where available.

case mutedStandard

A street map where MapKit emphasizes your data over the underlying map details.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing map properties

var isZoomEnabled: Bool

A Boolean value that determines whether the user may use pinch gestures to zoom in and out of the map.

var isScrollEnabled: Bool

A Boolean value that determines whether the user may scroll around the map.

var isPitchEnabled: Bool

A Boolean value that indicates whether the map uses the camera’s pitch information.

var isRotateEnabled: Bool

A Boolean value that indicates whether the map uses the camera’s heading information.

var mapType: MKMapType

The type of data the map view displays.

Deprecated

