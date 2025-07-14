

- MapKit
-  MKHybridMapConfiguration 

Class

# MKHybridMapConfiguration

The class that represents a satellite image of the area with road and road name information layers on top.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class MKHybridMapConfiguration
```

## Topics

### Creating a hybrid map configuration

init()

Creates a new hybrid map configuration.

convenience init(elevationStyle: MKMapConfiguration.ElevationStyle)

Creates a new hybrid map configuration with the specified elevation style.

enum ElevationStyle

Values that control the map’s elevation style.

### Controlling what the map displays

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter the framework uses to determine the points of interest to show on the map.

var showsTraffic: Bool

A Boolean value that indicates whether the maps shows traffic conditions.

## Relationships

### Inherits From

- MKMapConfiguration

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

class MKMapConfiguration

An abstract class that represents the shared elements of map configurations.

class MKStandardMapConfiguration

The class that represents the default map presentation, which is a street map that shows the position of all roads and some road names.

class MKImageryMapConfiguration

The class that represents an imagery-based map presentation, such as one using satellite imagery.

