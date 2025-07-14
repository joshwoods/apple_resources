

- MapKit
- MKScaleView
-  MKScaleView.Alignment 

Enumeration

# MKScaleView.Alignment

Constants indicating whether measurements begin at the leading or trailing edge of the view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
enum Alignment
```

## Topics

### Alignment options

case leading

Scale measurements begin at the leading edge of the view.

case trailing

Scale measurements begin at the trailing edge of the view.

case leading

Scale measurements begin at the leading edge of the view.

case trailing

Scale measurements begin at the trailing edge of the view.

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

### Getting the scale view attributes

var mapView: MKMapView?

The map view that provides the scale information to the scale view.

var scaleVisibility: MKFeatureVisibility

The visibility of the scale view.

var legendAlignment: MKScaleView.Alignment

The alignment of the distance information in the scale view.

