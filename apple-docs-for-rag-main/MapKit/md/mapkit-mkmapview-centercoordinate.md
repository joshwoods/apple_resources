

- MapKit
- MKMapView
-  centerCoordinate 

Instance Property

# centerCoordinate

The map coordinate at the center of the map view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var centerCoordinate: CLLocationCoordinate2D { get set }
```

## Discussion

Changing the value in this property centers the map on the new coordinate without changing the current zoom level. It also updates the values in the region property to reflect the new center coordinate and the new span values needed to maintain the current zoom level.

Changing the value of this property updates the map view immediately. If you want to animate the change, use the setCenter(_:animated:) method instead.

## See Also

### Manipulating the visible portion of the map

var region: MKCoordinateRegion

The area the map view displays.

func setRegion(MKCoordinateRegion, animated: Bool)

Changes the currently visible region, and optionally animates the change.

func setCenter(CLLocationCoordinate2D, animated: Bool)

Changes the center coordinate of the map, and optionally animates the change.

func showAnnotations([any MKAnnotation], animated: Bool)

Sets the visible region so that the map displays the specified annotations.

var visibleMapRect: MKMapRect

The area visible in the map view.

func setVisibleMapRect(MKMapRect, animated: Bool)

Changes the currently visible portion of the map, and optionally animates the change.

func setVisibleMapRect(MKMapRect, edgePadding: UIEdgeInsets, animated: Bool)

Changes the currently visible portion of the map, allowing you to specify additional space around the edges.

