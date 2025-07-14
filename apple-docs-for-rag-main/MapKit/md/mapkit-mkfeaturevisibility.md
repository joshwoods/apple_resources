

- MapKit
-  MKFeatureVisibility 

Enumeration

# MKFeatureVisibility

Constants that indicate the visibility of different map features.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

``` source
enum MKFeatureVisibility
```

## Topics

### Visibility options

case adaptive

A constant indicating that the feature adapts to the current map state.

case hidden

A constant indicating that the feature is hidden.

case visible

A constant indicating that the feature is visible.

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

### Getting the compass attributes

var mapView: MKMapView?

The map view that provides the heading information for the compass button.

var compassVisibility: MKFeatureVisibility

The visibility of the compass button.

