

- MapKit
- MKMapView
-  setCenter(\_:animated:) 

Instance Method

# setCenter(\_:animated:)

Changes the center coordinate of the map, and optionally animates the change.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func setCenter(
    _ coordinate: CLLocationCoordinate2D,
    animated: Bool
)
```

## Parameters 

`coordinate`  

The new center coordinate for the map.

`animated`  

Specify true if you want the map view to scroll to the new location or false if you want the map to display the new location immediately.

## Discussion

Changing the center coordinate centers the map on the new coordinate without changing the current zoom level. It also updates the value in the region property to reflect the new center coordinate and the new span values needed to maintain the current zoom level.

## See Also

### Manipulating the visible portion of the map

var region: MKCoordinateRegion

The area the map view displays.

func setRegion(MKCoordinateRegion, animated: Bool)

Changes the currently visible region, and optionally animates the change.

var centerCoordinate: CLLocationCoordinate2D

The map coordinate at the center of the map view.

func showAnnotations([any MKAnnotation], animated: Bool)

Sets the visible region so that the map displays the specified annotations.

var visibleMapRect: MKMapRect

The area visible in the map view.

func setVisibleMapRect(MKMapRect, animated: Bool)

Changes the currently visible portion of the map, and optionally animates the change.

func setVisibleMapRect(MKMapRect, edgePadding: UIEdgeInsets, animated: Bool)

Changes the currently visible portion of the map, allowing you to specify additional space around the edges.

