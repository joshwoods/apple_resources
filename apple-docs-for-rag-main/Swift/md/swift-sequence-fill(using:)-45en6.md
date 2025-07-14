

- Swift
- Sequence
-  fill(using:) 

Instance Method

# fill(using:)

Fills this list of rects in the current NSGraphicsContext with that rect’s associated color The compositing operation of the fill defaults to the context’s compositing operation, not necessarily using `.copy` like `NSRectFill()`.

macOS 10.9+Swift 4.0+

``` source
func fill(using operation: NSCompositingOperation = NSGraphicsContext.current?.compositingOperation ?? .sourceOver)
```

Available when `Element` is `(CGRect, NSColor)`.

## Discussion

Precondition

There must be a set current NSGraphicsContext.

## See Also

### Applying AppKit Graphic Operations

func fill(using: NSCompositingOperation)

Fills this list of rects in the current NSGraphicsContext in the context’s fill color. The compositing operation of the fill defaults to the context’s compositing operation, not necessarily using `.copy` like `NSRectFill()`.

func clip()

Modifies the current graphics context clipping path by intersecting it with the graphical union of this list of rects This permanently modifies the graphics state, so the current state should be saved beforehand and restored afterwards.

