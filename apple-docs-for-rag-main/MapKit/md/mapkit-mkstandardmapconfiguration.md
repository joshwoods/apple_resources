

- MapKit
-  MKStandardMapConfiguration 

Class

# MKStandardMapConfiguration

The class that represents the default map presentation, which is a street map that shows the position of all roads and some road names.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class MKStandardMapConfiguration
```

## Topics

### Creating a standard map configuration

init()

Creates a new standard map configuration.

convenience init(elevationStyle: MKMapConfiguration.ElevationStyle)

Creates a new standard map configuration with the specified elevation style.

convenience init(elevationStyle: MKMapConfiguration.ElevationStyle, emphasisStyle: MKStandardMapConfiguration.EmphasisStyle)

Creates a standard map configuration with the specified elevation and emphasis styles.

convenience init(emphasisStyle: MKStandardMapConfiguration.EmphasisStyle)

Creates a standard map configuration with the specified emphasis style.

enum ElevationStyle

Values that control the map’s elevation style.

enum EmphasisStyle

Values that control how the framework emphasizes map features.

### Customizing the map display

var emphasisStyle: MKStandardMapConfiguration.EmphasisStyle

The value that indicates how the framework emphasizes map features.

enum EmphasisStyle

Values that control how the framework emphasizes map features.

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter used to determine the points of interest shown on the map.

var showsTraffic: Bool

A Boolean value that controls whether the map displays traffic conditions.

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

class MKHybridMapConfiguration

The class that represents a satellite image of the area with road and road name information layers on top.

class MKImageryMapConfiguration

The class that represents an imagery-based map presentation, such as one using satellite imagery.

