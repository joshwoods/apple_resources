

- MapKit
-  MKMapConfiguration 

Class

# MKMapConfiguration

An abstract class that represents the shared elements of map configurations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class MKMapConfiguration
```

## Topics

### Controlling the elevation style

var elevationStyle: MKMapConfiguration.ElevationStyle

The value that indicates the map’s elevation style.

enum ElevationStyle

Values that control the map’s elevation style.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MKHybridMapConfiguration
- MKImageryMapConfiguration
- MKStandardMapConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Configuring the map appearance

var preferredConfiguration: MKMapConfiguration

The characteristics of the map view, including the map type and features the map displays.

var pitchButtonVisibility: MKFeatureVisibility

A value that indicates whether the map’s pitch button is visible.

var showsUserTrackingButton: Bool

A Boolean value that indicates whether the map displays the user tracking button.

class MKStandardMapConfiguration

The class that represents the default map presentation, which is a street map that shows the position of all roads and some road names.

class MKHybridMapConfiguration

The class that represents a satellite image of the area with road and road name information layers on top.

class MKImageryMapConfiguration

The class that represents an imagery-based map presentation, such as one using satellite imagery.

