

- MapKit
- MKScaleView
-  init(mapView:) 

Initializer

# init(mapView:)

Creates a scale view and associates it with the specified map view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
convenience init(mapView: MKMapView?)
```

## Parameters 

`mapView`  

The map to associate with the scale view. The scale view automatically updates to reflect the scale of this map.

## Return Value

An initialized scale view.

