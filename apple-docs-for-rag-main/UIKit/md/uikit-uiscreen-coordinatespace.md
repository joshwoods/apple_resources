

- UIKit
- UIScreen
-  coordinateSpace 

Instance Property

# coordinateSpace

The current coordinate space of the screen.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var coordinateSpace: any UICoordinateSpace { get }
```

## Discussion

The screen’s current coordinate space always reflects any interface orientations applied to the device. Therefore, the bounds of this coordinate space match the bounds property of the screen itself.

## See Also

### Getting the coordinate space

var fixedCoordinateSpace: any UICoordinateSpace

The fixed coordinate space of the screen.

