

- MapKit
- MapContent
-  mapOverlayLevel(level:) 

Instance Method

# mapOverlayLevel(level:)

Specifies the position of overlays relative to other map content.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
func mapOverlayLevel(level: MKOverlayLevel) -> some MapContent
```

## Parameters 

`level`  

One of the MKOverlayLevel levels.

## Return Value

Returns MapContent with overlays drawn with the positioning level you specified.

