

- MapKit
- MKOverlayRenderer
-  init(overlay:) 

Initializer

# init(overlay:)

Creates and returns the overlay renderer and associates it with the specified overlay object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
init(overlay: any MKOverlay)
```

## Parameters 

`overlay`  

The overlay object to use when drawing the overlay content on the map. This object provides the data needed to draw the overlay’s shape. The overlay renderer stores a strong reference to this object.

## Return Value

An initialized overlay renderer object.

## Discussion

Initially, the overlay renderer assumes that the overlay is fully opaque and that it has a content scale factor of 1.0. You can change these values as needed using the alpha and contentScaleFactor properties.

