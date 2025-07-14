

- MapKit
- MKMapView
-  preferredConfiguration 

Instance Property

# preferredConfiguration

The characteristics of the map view, including the map type and features the map displays.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var preferredConfiguration: MKMapConfiguration { get set }
```

## See Also

### Configuring the map appearance

var pitchButtonVisibility: MKFeatureVisibility

A value that indicates whether the map’s pitch button is visible.

var showsUserTrackingButton: Bool

A Boolean value that indicates whether the map displays the user tracking button.

class MKMapConfiguration

An abstract class that represents the shared elements of map configurations.

class MKStandardMapConfiguration

The class that represents the default map presentation, which is a street map that shows the position of all roads and some road names.

class MKHybridMapConfiguration

The class that represents a satellite image of the area with road and road name information layers on top.

class MKImageryMapConfiguration

The class that represents an imagery-based map presentation, such as one using satellite imagery.

