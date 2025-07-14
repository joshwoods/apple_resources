

- MapKit
- MKMapViewDelegate
-  mapView(\_:rendererFor:) 

Instance Method

# mapView(\_:rendererFor:)

Asks the delegate for a renderer object to use when drawing the specified overlay.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    rendererFor overlay: any MKOverlay
) -> MKOverlayRenderer
```

## Parameters 

`mapView`  

The map view that requests the renderer object.

`overlay`  

The overlay object that the map view is about to display.

## Return Value

The renderer to use when presenting the specified overlay on the map.

## Discussion

Implement this method and use it to provide an appropriate renderer object for your overlays. The renderer object is responsible for drawing the contents of your overlay when the map view requests it to. MapKit supports many different types of standard renderer objects and you may also define your own custom renderers.

## See Also

### Managing the display of overlays

func mapView(MKMapView, selectionAccessoryFor: any MKAnnotation) -> MKSelectionAccessory?

Specifies the accessory to display for a selected annotation

func mapView(MKMapView, didAdd: [MKOverlayRenderer])

Tells the delegate when the map view adds one or more renderer objects to the map.

func mapView(MKMapView, viewFor: any MKOverlay) -> MKOverlayView

Asks the delegate for the overlay view to use when displaying the specified overlay object.

Deprecated

func mapView(MKMapView, didAddOverlayViews: [Any])

Tells the delegate when the map adds one or more overlay views to the map.

Deprecated

