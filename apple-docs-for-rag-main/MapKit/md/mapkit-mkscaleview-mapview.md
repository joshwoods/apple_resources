

- MapKit
- MKScaleView
-  mapView 

Instance Property

# mapView

The map view that provides the scale information to the scale view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
weak var mapView: MKMapView? { get set }
```

## See Also

### Getting the scale view attributes

var scaleVisibility: MKFeatureVisibility

The visibility of the scale view.

var legendAlignment: MKScaleView.Alignment

The alignment of the distance information in the scale view.

enum Alignment

Constants indicating whether measurements begin at the leading or trailing edge of the view.

