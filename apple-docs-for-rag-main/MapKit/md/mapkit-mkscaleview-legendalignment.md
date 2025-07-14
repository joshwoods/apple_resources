

- MapKit
- MKScaleView
-  legendAlignment 

Instance Property

# legendAlignment

The alignment of the distance information in the scale view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var legendAlignment: MKScaleView.Alignment { get set }
```

## Discussion

This property determines whether measurements start at the leading or trailing edge of the view. The default value of this property is MKScaleView.Alignment.leading.

## See Also

### Getting the scale view attributes

var mapView: MKMapView?

The map view that provides the scale information to the scale view.

var scaleVisibility: MKFeatureVisibility

The visibility of the scale view.

enum Alignment

Constants indicating whether measurements begin at the leading or trailing edge of the view.

