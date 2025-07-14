

- MapKit
- MKCompassButton
-  compassVisibility 

Instance Property

# compassVisibility

The visibility of the compass button.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
var compassVisibility: MKFeatureVisibility { get set }
```

## Discussion

You can configure a compass button to be visible all the time or only when the compass heading changes.

## See Also

### Getting the compass attributes

var mapView: MKMapView?

The map view that provides the heading information for the compass button.

enum MKFeatureVisibility

Constants that indicate the visibility of different map features.

