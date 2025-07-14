

- MapKit
- MKMapView
-  showsUserTrackingButton 

Instance Property

# showsUserTrackingButton

A Boolean value that indicates whether the map displays the user tracking button.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var showsUserTrackingButton: Bool { get set }
```

## See Also

### Configuring the map appearance

var preferredConfiguration: MKMapConfiguration

The characteristics of the map view, including the map type and features the map displays.

var pitchButtonVisibility: MKFeatureVisibility

A value that indicates whether the map’s pitch button is visible.

class MKMapConfiguration

An abstract class that represents the shared elements of map configurations.

class MKStandardMapConfiguration

The class that represents the default map presentation, which is a street map that shows the position of all roads and some road names.

class MKHybridMapConfiguration

The class that represents a satellite image of the area with road and road name information layers on top.

class MKImageryMapConfiguration

The class that represents an imagery-based map presentation, such as one using satellite imagery.

