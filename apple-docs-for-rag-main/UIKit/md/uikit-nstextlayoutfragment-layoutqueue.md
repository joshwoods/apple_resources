

- UIKit
- NSTextLayoutFragment
-  layoutQueue 

Instance Property

# layoutQueue

The queue on which the framework dispatches layout operations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var layoutQueue: OperationQueue? { get set }
```

## Discussion

If non-`nil`, the queue the framework uses for layout operations.

