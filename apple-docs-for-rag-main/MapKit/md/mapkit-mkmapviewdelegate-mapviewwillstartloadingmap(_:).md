

- MapKit
- MKMapViewDelegate
-  mapViewWillStartLoadingMap(\_:) 

Instance Method

# mapViewWillStartLoadingMap(\_:)

Tells the delegate that the specified map view is about to retrieve some map data.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapViewWillStartLoadingMap(_ mapView: MKMapView)
```

## Parameters 

`mapView`  

The map view that begins loading the data.

## Discussion

The map view calls this method whenever it needs to download a new group of map tiles from the server. This typically occurs whenever you expose portions of the map by panning or zooming the content. You can use this method to mark the time that it takes for the map view to load the data.

## See Also

### Loading the map data

func mapViewDidFinishLoadingMap(MKMapView)

Tells the delegate when the specified map view successfully loads the needed map data.

func mapViewDidFailLoadingMap(MKMapView, withError: any Error)

Tells the delegate that the specified view is unable to load the map data.

func mapViewWillStartRenderingMap(MKMapView)

Tells the delegate that the map view is about to start rendering some of its tiles.

func mapViewDidFinishRenderingMap(MKMapView, fullyRendered: Bool)

Tells the delegate when the map view finishes rendering all visible tiles.

