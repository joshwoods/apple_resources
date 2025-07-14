

- MapKit
- MKMapViewDelegate
-  mapViewDidFailLoadingMap(\_:withError:) 

Instance Method

# mapViewDidFailLoadingMap(\_:withError:)

Tells the delegate that the specified view is unable to load the map data.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapViewDidFailLoadingMap(
    _ mapView: MKMapView,
    withError error: any Error
)
```

## Parameters 

`mapView`  

The map view that starts the load operation.

`error`  

The reason that the map view can’t load the map data.

## Discussion

The map view might call this method in situations where the device doesn’t have access to the network or is unable to load the map data for some reason. The map view may also call this method if a request for additional map tiles comes in while a previous request for tiles is pending. You can use this message to notify the user that the map data is unavailable.

## See Also

### Loading the map data

func mapViewWillStartLoadingMap(MKMapView)

Tells the delegate that the specified map view is about to retrieve some map data.

func mapViewDidFinishLoadingMap(MKMapView)

Tells the delegate when the specified map view successfully loads the needed map data.

func mapViewWillStartRenderingMap(MKMapView)

Tells the delegate that the map view is about to start rendering some of its tiles.

func mapViewDidFinishRenderingMap(MKMapView, fullyRendered: Bool)

Tells the delegate when the map view finishes rendering all visible tiles.

