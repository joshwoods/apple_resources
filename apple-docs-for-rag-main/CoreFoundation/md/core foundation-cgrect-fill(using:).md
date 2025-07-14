

- Core Foundation
- CGRect
-  fill(using:) 

Instance Method

# fill(using:)

Fills this rect in the current NSGraphicsContext in the context’s fill color. The compositing operation of the fill defaults to the context’s compositing operation, not necessarily using `.copy` like `NSRectFill()`.

macOS 10.9+Swift 4.0+

``` source
func fill(using operation: NSCompositingOperation = NSGraphicsContext.current?.compositingOperation ?? .sourceOver)
```

## Discussion

Precondition

There must be a set current NSGraphicsContext.

