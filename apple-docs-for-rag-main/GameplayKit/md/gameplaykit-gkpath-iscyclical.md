

- GameplayKit
- GKPath
-  isCyclical 

Instance Property

# isCyclical

A Boolean value that determines whether the path loops around on itself (that is, the path’s end point connects to its start point).

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var isCyclical: Bool { get set }
```

## Discussion

When you create a path with the initWithPoints:count:radius:cyclical: or pathWithPoints:count:radius:cyclical: method, the order of vectors in the `points` parameter determines the order in which an agent with a path-following goal traverses the path. If the path is not cyclical, an agent traversing the path will stop at the end point. If the path is cyclical, the agent will loop around to the start point and continue following the path indefinitely.

## See Also

### Managing a Path’s Attributes

var radius: Float

The radius of the path.

