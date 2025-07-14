

- MapKit
- MKScaleView
-  scaleVisibility 

Instance Property

# scaleVisibility

The visibility of the scale view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var scaleVisibility: MKFeatureVisibility { get set }
```

## Discussion

You can configure a scale view to be visible all the time or only when the scale of the map changes.

## See Also

### Getting the scale view attributes

var mapView: MKMapView?

The map view that provides the scale information to the scale view.

var legendAlignment: MKScaleView.Alignment

The alignment of the distance information in the scale view.

enum Alignment

Constants indicating whether measurements begin at the leading or trailing edge of the view.

