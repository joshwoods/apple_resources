

- Core Foundation
- CGRect
-  frame(withWidth:using:) 

Instance Method

# frame(withWidth:using:)

Draws a frame around the inside of this rect in the current NSGraphicsContext in the context’s fill color The compositing operation of the fill defaults to the context’s compositing operation, not necessarily using `.copy` like `NSFrameRect()`.

macOS 10.9+Swift 4.0+

``` source
func frame(
    withWidth width: CGFloat = 1.0,
    using operation: NSCompositingOperation = NSGraphicsContext.current?.compositingOperation ?? .sourceOver
)
```

## Discussion

Precondition

There must be a set current NSGraphicsContext.

