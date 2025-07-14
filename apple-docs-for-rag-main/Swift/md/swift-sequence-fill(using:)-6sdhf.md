

- Swift
- Sequence
-  fill(using:) 

Instance Method

# fill(using:)

Fills this list of rects in the current NSGraphicsContext with that rect’s associated gray component value in the DeviceGray color space. The compositing operation of the fill defaults to the context’s compositing operation, not necessarily using `.copy` like `NSRectFillListWithGrays()`.

macOS 10.9+Swift 4.0+

``` source
func fill(using operation: NSCompositingOperation = NSGraphicsContext.current?.compositingOperation ?? .sourceOver)
```

Available when `Element` is `(CGRect, gray: CGFloat)`.

## Discussion

Precondition

There must be a set current NSGraphicsContext.

