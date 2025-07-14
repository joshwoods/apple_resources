

- MapKit
- MKUserTrackingButton
-  init(mapView:) 

Initializer

# init(mapView:)

Initializes the button with the map view that it should control.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(mapView: MKMapView?)
```

## Parameters 

`mapView`  

The mapView to associate with the button. Taps on the button change the appearance of this map view.

## Return Value

An initialized MKUserTrackingButton object.

