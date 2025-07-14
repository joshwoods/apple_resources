

- MapKit
- MKCompassButton
-  init(mapView:) 

Initializer

# init(mapView:)

Creates a compass button and associates it with the specified map view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
convenience init(mapView: MKMapView?)
```

## Parameters 

`mapView`  

The map to associate with the compass button. The compass button reflects the orientation of this map, and tapping the button reorients the map appropriately.

## Return Value

An initialized compass button.

