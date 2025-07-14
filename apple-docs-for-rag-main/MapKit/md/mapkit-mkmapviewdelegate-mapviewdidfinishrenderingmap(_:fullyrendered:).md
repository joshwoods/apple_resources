

- MapKit
- MKMapViewDelegate
-  mapViewDidFinishRenderingMap(\_:fullyRendered:) 

Instance Method

# mapViewDidFinishRenderingMap(\_:fullyRendered:)

Tells the delegate when the map view finishes rendering all visible tiles.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapViewDidFinishRenderingMap(
    _ mapView: MKMapView,
    fullyRendered: Bool
)
```

## Parameters 

`mapView`  

The map view rendering its tiles.

`fullyRendered`  

This parameter is true if the map view is able to render all tiles completely, or false if errors prevent the map view from rendering all tiles.

## Discussion

This method lets you know when the map view finishes rendering all of the currently visible tiles to the best of its ability. The map view calls this method regardless of whether the view renders all tiles successfully. If there are errors loading one or more tiles that prevent the map view from rendering them, MapKit sets the `fullyRendered` parameter to false.

## See Also

### Loading the map data

func mapViewWillStartLoadingMap(MKMapView)

Tells the delegate that the specified map view is about to retrieve some map data.

func mapViewDidFinishLoadingMap(MKMapView)

Tells the delegate when the specified map view successfully loads the needed map data.

func mapViewDidFailLoadingMap(MKMapView, withError: any Error)

Tells the delegate that the specified view is unable to load the map data.

func mapViewWillStartRenderingMap(MKMapView)

Tells the delegate that the map view is about to start rendering some of its tiles.

