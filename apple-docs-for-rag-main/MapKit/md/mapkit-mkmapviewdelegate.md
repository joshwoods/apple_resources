

- MapKit
-  MKMapViewDelegate 

Protocol

# MKMapViewDelegate

Optional methods that you use to receive map-related update messages.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
protocol MKMapViewDelegate : NSObjectProtocol
```

## Overview

Because many map operations require the MKMapView class to load data asynchronously, the map view calls these methods to notify your app when specific operations complete. The map view also uses these methods to request annotation and overlay views, and to manage interactions with those views.

Before releasing an MKMapView object that you set a delegate for, remember to set that object’s delegate property to `nil`. MapKit calls all of your delegate methods on the app’s main thread.

## Topics

### Responding to map position changes

func mapView(MKMapView, regionWillChangeAnimated: Bool)

Tells the delegate when the region the map view is displaying is about to change.

func mapViewDidChangeVisibleRegion(MKMapView)

Tells the delegate when the map view’s visible region changes.

func mapView(MKMapView, regionDidChangeAnimated: Bool)

Tells the delegate when the region the map view is displaying changes.

### Loading the map data

func mapViewWillStartLoadingMap(MKMapView)

Tells the delegate that the specified map view is about to retrieve some map data.

func mapViewDidFinishLoadingMap(MKMapView)

Tells the delegate when the specified map view successfully loads the needed map data.

func mapViewDidFailLoadingMap(MKMapView, withError: any Error)

Tells the delegate that the specified view is unable to load the map data.

func mapViewWillStartRenderingMap(MKMapView)

Tells the delegate that the map view is about to start rendering some of its tiles.

func mapViewDidFinishRenderingMap(MKMapView, fullyRendered: Bool)

Tells the delegate when the map view finishes rendering all visible tiles.

### Tracking the user’s location

func mapViewWillStartLocatingUser(MKMapView)

Tells the delegate that the map view is about to start tracking the user’s location.

func mapViewDidStopLocatingUser(MKMapView)

Tells the delegate when the map view stops tracking the user’s location.

func mapView(MKMapView, didUpdate: MKUserLocation)

Tells the delegate when the map view updates the user’s location.

func mapView(MKMapView, didFailToLocateUserWithError: any Error)

Tells the delegate when an attempt to locate the user’s location fails.

func mapView(MKMapView, didChange: MKUserTrackingMode, animated: Bool)

Tells the delegate when the user-tracking mode changes.

### Managing annotation views

func mapView(MKMapView, viewFor: any MKAnnotation) -> MKAnnotationView?

Returns the view associated with the specified annotation object.

func mapView(MKMapView, didAdd: [MKAnnotationView])

Tells the delegate when the map view adds one or more annotation views to the map.

func mapView(MKMapView, annotationView: MKAnnotationView, calloutAccessoryControlTapped: UIControl)

Tells the delegate when the user taps one of the annotation view’s accessory buttons.

func mapView(MKMapView, clusterAnnotationForMemberAnnotations: [any MKAnnotation]) -> MKClusterAnnotation

Asks the delegate to provide a cluster annotation object for the specified annotations.

### Dragging an annotation view

func mapView(MKMapView, annotationView: MKAnnotationView, didChange: MKAnnotationView.DragState, fromOldState: MKAnnotationView.DragState)

Tells the delegate when the drag state of one of its annotation views changes.

### Selecting annotations and annotations views

func mapView(MKMapView, didSelect: MKAnnotationView)

Tells the delegate when the user selects one or more of its annotation views.

func mapView(MKMapView, didDeselect: MKAnnotationView)

Tells the delegate when the user deselects one or more of its annotation views.

func mapView(MKMapView, didDeselect: any MKAnnotation)

Tells the delegate when the user deselects one or more annotations.

func mapView(MKMapView, didSelect: any MKAnnotation)

Tells the delegate when the user selects one or more annotations.

var selectableMapFeatures: MKMapFeatureOptions

The property that describes which selectable features the map responds to.

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

func mapView(MKMapView, didAddOverlayViews: [Any])

Tells the delegate when the map adds one or more overlay views to the map.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Customizing the map view behavior

var delegate: (any MKMapViewDelegate)?

The receiver’s delegate.

