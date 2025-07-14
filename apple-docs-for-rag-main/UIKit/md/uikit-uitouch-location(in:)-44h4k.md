

- UIKit
- UITouch
-  location(in:) 

Instance Method

# location(in:)

Returns the current location of the touch in the coordinate system of the given node.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func location(in node: SKNode) -> CGPoint
```

## Parameters 

`node`  

A node that is a descendant of a scene presented in the window that received the touch event.

## Return Value

The location of the touch in the node’s coordinate system.

## See Also

### Working with touch events in SpriteKit

func previousLocation(in: SKNode) -> CGPoint

Returns the previous location of the touch in the coordinate system of the given node.

