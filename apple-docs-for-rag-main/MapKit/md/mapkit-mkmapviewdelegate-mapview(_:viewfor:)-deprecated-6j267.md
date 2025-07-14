

- MapKit
- MKMapViewDelegate
-  mapView(\_:viewFor:) Deprecated

Instance Method

# mapView(\_:viewFor:)

Asks the delegate for the overlay view to use when displaying the specified overlay object.

iOS 4.0–13.0DeprecatediPadOS 4.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    viewFor overlay: any MKOverlay
) -> MKOverlayView
```

Deprecated

Implement the mapView(_:rendererFor:) method instead.

## Parameters 

`mapView`  

The map view that requests the overlay view.

`overlay`  

The object representing the overlay that the map view is about to display.

## Return Value

The view to use when presenting the specified overlay on the map. If you return `nil`, no view displays for the specified overlay object.

## See Also

### Managing the display of overlays

func mapView(MKMapView, selectionAccessoryFor: any MKAnnotation) -> MKSelectionAccessory?

Specifies the accessory to display for a selected annotation

func mapView(MKMapView, rendererFor: any MKOverlay) -> MKOverlayRenderer

Asks the delegate for a renderer object to use when drawing the specified overlay.

func mapView(MKMapView, didAdd: [MKOverlayRenderer])

Tells the delegate when the map view adds one or more renderer objects to the map.

func mapView(MKMapView, didAddOverlayViews: [Any])

Tells the delegate when the map adds one or more overlay views to the map.

Deprecated

