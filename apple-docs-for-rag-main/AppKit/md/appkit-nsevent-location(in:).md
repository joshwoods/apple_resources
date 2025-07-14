

- AppKit
- NSEvent
-  location(in:) 

Instance Method

# location(in:)

Returns the location of the receiver in the coordinate system of the given node.

macOS

``` source
func location(in node: SKNode) -> CGPoint
```

## Parameters 

`node`  

A node that is a descendant of a scene presented in the window that received the mouse event.

## Return Value

The location of the event in the node’s coordinate system.

