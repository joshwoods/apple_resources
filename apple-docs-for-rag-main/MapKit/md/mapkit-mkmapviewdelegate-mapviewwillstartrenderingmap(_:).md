

- MapKit
- MKMapViewDelegate
-  mapViewWillStartRenderingMap(\_:) 

Instance Method

# mapViewWillStartRenderingMap(\_:)

Tells the delegate that the map view is about to start rendering some of its tiles.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapViewWillStartRenderingMap(_ mapView: MKMapView)
```

## Parameters 

`mapView`  

The map view that’s about to start rendering.

## Discussion

The map view calls this method when the map reveals one or more tiles that require rendering.

## See Also

### Loading the map data

func mapViewWillStartLoadingMap(MKMapView)

Tells the delegate that the specified map view is about to retrieve some map data.

func mapViewDidFinishLoadingMap(MKMapView)

Tells the delegate when the specified map view successfully loads the needed map data.

func mapViewDidFailLoadingMap(MKMapView, withError: any Error)

Tells the delegate that the specified view is unable to load the map data.

func mapViewDidFinishRenderingMap(MKMapView, fullyRendered: Bool)

Tells the delegate when the map view finishes rendering all visible tiles.

