

- MapKit
- MKMapViewDelegate
-  mapView(\_:selectionAccessoryFor:) 

Instance Method

# mapView(\_:selectionAccessoryFor:)

Specifies the accessory to display for a selected annotation

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    selectionAccessoryFor annotation: any MKAnnotation
) -> MKSelectionAccessory?
```

## Parameters 

`mapView`  

The map view that requests the selection accessory.

`annotation`  

The annotation.

## Discussion

Called for all selected annotations. Not all types of annotations support displaying selection accessories. For example, the map item detail selection accessory is only supported for MKMapItemAnnotation and MKMapFeatureAnnotation. Please return \`nil\` for annotations where a selection accessory is not desired.

No accessory will be displayed if…

- nil is returned

- mapView(_:selectionAccessoryFor:) is not implemented

- the accessory returned is not supported for \`annotation\`

## See Also

### Managing the display of overlays

func mapView(MKMapView, rendererFor: any MKOverlay) -> MKOverlayRenderer

Asks the delegate for a renderer object to use when drawing the specified overlay.

func mapView(MKMapView, didAdd: [MKOverlayRenderer])

Tells the delegate when the map view adds one or more renderer objects to the map.

func mapView(MKMapView, viewFor: any MKOverlay) -> MKOverlayView

Asks the delegate for the overlay view to use when displaying the specified overlay object.

Deprecated

func mapView(MKMapView, didAddOverlayViews: [Any])

Tells the delegate when the map adds one or more overlay views to the map.

Deprecated

