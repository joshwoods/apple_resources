

- MapKit
- MKMapView
-  removeOverlay(\_:) 

Instance Method

# removeOverlay(\_:)

Removes a single overlay object from the map.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func removeOverlay(_ overlay: any MKOverlay)
```

## Parameters 

`overlay`  

The overlay object to remove.

## Discussion

This method removes the overlay regardless of the level that it’s in. Removing an overlay also removes its corresponding renderer, if one is in use. If the specified overlay isn’t associated with the map view, this method does nothing.

## See Also

### Related Documentation

func addOverlay(any MKOverlay)

Adds a single overlay object to the map.

func addOverlays([any MKOverlay])

Adds an array of overlay objects to the map.

### Removing overlays

func removeOverlays([any MKOverlay])

Removes one or more overlay objects from the map.

