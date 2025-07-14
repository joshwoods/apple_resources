

- MapKit
- MKMapViewDelegate
-  mapView(\_:didAddOverlayViews:) Deprecated

Instance Method

# mapView(\_:didAddOverlayViews:)

Tells the delegate when the map adds one or more overlay views to the map.

iOS 4.0–13.0DeprecatediPadOS 4.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    didAddOverlayViews overlayViews: [Any]
)
```

Deprecated

Implement the mapView(_:didAdd:) method instead.

## Parameters 

`mapView`  

The map view that adds the overlay views.

`overlayViews`  

An array of MKOverlayView objects representing the views that the map view adds.

## Discussion

By the time the map view calls this method, MapKit has added the specified views to the map.

## See Also

### Managing the display of overlays

func mapView(MKMapView, selectionAccessoryFor: any MKAnnotation) -> MKSelectionAccessory?

Specifies the accessory to display for a selected annotation

func mapView(MKMapView, rendererFor: any MKOverlay) -> MKOverlayRenderer

Asks the delegate for a renderer object to use when drawing the specified overlay.

func mapView(MKMapView, didAdd: [MKOverlayRenderer])

Tells the delegate when the map view adds one or more renderer objects to the map.

func mapView(MKMapView, viewFor: any MKOverlay) -> MKOverlayView

Asks the delegate for the overlay view to use when displaying the specified overlay object.

Deprecated

