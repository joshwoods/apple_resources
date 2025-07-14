

- AppKit
- NSTextLayoutFragment
-  layoutQueue 

Instance Property

# layoutQueue

The queue on which the framework dispatches layout operations.

macOS 12.0+

``` source
var layoutQueue: OperationQueue? { get set }
```

## Discussion

If non-`nil`, the queue the framework uses for layout operations.

