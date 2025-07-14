

- MapKit
- MKMapViewDelegate
-  mapView(\_:didAdd:) 

Instance Method

# mapView(\_:didAdd:)

Tells the delegate when the map view adds one or more renderer objects to the map.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    didAdd renderers: [MKOverlayRenderer]
)
```

## Parameters 

`mapView`  

The map view that adds the renderer objects.

`renderers`  

The renderer objects that the map view adds.

## Discussion

The map view adds renderer objects when it needs them to draw their contents, which might be prior to those contents appearing onscreen. It calls this method to let you know that the renderer is active and in use. By the time the map view calls this method, it has already added specified renderers to the map.

## See Also

### Managing the display of overlays

func mapView(MKMapView, selectionAccessoryFor: any MKAnnotation) -> MKSelectionAccessory?

Specifies the accessory to display for a selected annotation

func mapView(MKMapView, rendererFor: any MKOverlay) -> MKOverlayRenderer

Asks the delegate for a renderer object to use when drawing the specified overlay.

func mapView(MKMapView, viewFor: any MKOverlay) -> MKOverlayView

Asks the delegate for the overlay view to use when displaying the specified overlay object.

Deprecated

func mapView(MKMapView, didAddOverlayViews: [Any])

Tells the delegate when the map adds one or more overlay views to the map.

Deprecated

