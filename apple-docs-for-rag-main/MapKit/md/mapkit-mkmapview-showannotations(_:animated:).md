

- MapKit
- MKMapView
-  showAnnotations(\_:animated:) 

Instance Method

# showAnnotations(\_:animated:)

Sets the visible region so that the map displays the specified annotations.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func showAnnotations(
    _ annotations: [any MKAnnotation],
    animated: Bool
)
```

## Parameters 

`annotations`  

The annotations that you want to be visible on the map.

`animated`  

Specify true if you want the map view to animate the region change, or false if you want the map to display the new region immediately without animations.

## Discussion

Calling this method updates the value in the region property, and potentially other properties, to reflect the new map region.

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

var visibleMapRect: MKMapRect

The area visible in the map view.

func setVisibleMapRect(MKMapRect, animated: Bool)

Changes the currently visible portion of the map, and optionally animates the change.

func setVisibleMapRect(MKMapRect, edgePadding: UIEdgeInsets, animated: Bool)

Changes the currently visible portion of the map, allowing you to specify additional space around the edges.

