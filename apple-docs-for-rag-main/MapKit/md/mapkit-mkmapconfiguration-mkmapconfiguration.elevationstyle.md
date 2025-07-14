

- MapKit
- MKMapConfiguration
-  MKMapConfiguration.ElevationStyle 

Enumeration

# MKMapConfiguration.ElevationStyle

Values that control the map’s elevation style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum ElevationStyle
```

## Topics

### Constants

case flat

The value that represents the flat map elevation style.

case realistic

The value that represents a map elevation style with realistic ground contours.

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

### Creating a hybrid map configuration

init()

Creates a new hybrid map configuration.

convenience init(elevationStyle: MKMapConfiguration.ElevationStyle)

Creates a new hybrid map configuration with the specified elevation style.

