

- MapKit
- MKMapView
-  region 

Instance Property

# region

The area the map view displays.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var region: MKCoordinateRegion { get set }
```

## Discussion

The *region* encompasses both the latitude and longitude center point of the map, and the span of coordinates to display. The span values provide an implicit zoom value for the map. The larger the displayed area, the lower the amount of zoom. Similarly, the smaller the displayed area, the greater the amount of zoom.

Changing only the center coordinate of the region can still cause the span to change implicitly. The span might change because the distances that a span represents change at different latitudes and longitudes, and the map view may need to adjust the span to account for the new location. If you want to change the center coordinate without changing the zoom level, use the centerCoordinate instead.

Changing the value of this property updates the map view immediately. When setting this property, the map may adjust the new region value so that it fits the visible area of the map precisely. This ensures that the value in this property reflects the visible portion of the map. However, it does mean that if you get the value of this property right after setting it, the returned value may not match the value you set. You can use the regionThatFits(_:) method to determine the region that the map sets.

If you want to animate the change in region, use the setRegion(_:animated:) method instead.

## See Also

### Manipulating the visible portion of the map

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

func setVisibleMapRect(MKMapRect, animated: Bool)

Changes the currently visible portion of the map, and optionally animates the change.

func setVisibleMapRect(MKMapRect, edgePadding: UIEdgeInsets, animated: Bool)

Changes the currently visible portion of the map, allowing you to specify additional space around the edges.

