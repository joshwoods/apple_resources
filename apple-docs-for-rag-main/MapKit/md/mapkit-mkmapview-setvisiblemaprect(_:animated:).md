

- MapKit
- MKMapView
-  setVisibleMapRect(\_:animated:) 

Instance Method

# setVisibleMapRect(\_:animated:)

Changes the currently visible portion of the map, and optionally animates the change.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func setVisibleMapRect(
    _ mapRect: MKMapRect,
    animated animate: Bool
)
```

## Parameters 

`mapRect`  

The map rectangle to make visible in the map view.

`animate`  

Specify true if you want the map view to animate the transition to the new map rectangle or false if you want the map to center on the specified rectangle immediately.

## See Also

### Manipulating the visible portion of the map

var region: MKCoordinateRegion

The area the map view displays.

func setRegion(MKCoordinateRegion, animated: Bool)

Changes the currently visible region, and optionally animates the change.

var centerCoordinate: CLLocationCoordinate2D

The map coordinate at the center of the map view.

func setCenter(CLLocationCoordinate2D, animated: Bool)

Changes the center coordinate of the map, and optionally animates the change.

func showAnnotations([any MKAnnotation], animated: Bool)

Sets the visible region so that the map displays the specified annotations.

var visibleMapRect: MKMapRect

The area visible in the map view.

func setVisibleMapRect(MKMapRect, edgePadding: UIEdgeInsets, animated: Bool)

Changes the currently visible portion of the map, allowing you to specify additional space around the edges.

