

- MapKit
- MKMapView
-  removeOverlays(\_:) 

Instance Method

# removeOverlays(\_:)

Removes one or more overlay objects from the map.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func removeOverlays(_ overlays: [any MKOverlay])
```

## Parameters 

`overlays`  

An array of objects, each of which conforms to the MKOverlay protocol.

## Discussion

This method removes the specified overlays regardless of which level each one is in. Removing an overlay also removes its corresponding renderer, if one is in use. The method ignores an overlay object if it isn’t associated with the map view.

## See Also

### Related Documentation

func addOverlay(any MKOverlay)

Adds a single overlay object to the map.

func addOverlays([any MKOverlay])

Adds an array of overlay objects to the map.

### Removing overlays

func removeOverlay(any MKOverlay)

Removes a single overlay object from the map.

