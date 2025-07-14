

- AppKit
- NSGraphicsContext
-  restoreGraphicsState() 

Type Method

# restoreGraphicsState()

Pops a graphics context from the per-thread stack, makes it current, and sends the context a restore graphics state message.

macOS

``` source
class func restoreGraphicsState()
```

## See Also

### Managing the Graphics State

func restoreGraphicsState()

Removes the context’s graphics state from the top of the graphics state stack and makes the next graphics state the current graphics state.

class func saveGraphicsState()

Saves the graphics state of the current graphics context.

func saveGraphicsState()

Saves the current graphics state and creates a new graphics state on the top of the stack.

class func setGraphicsState(Int)

Makes the graphics context of the specified graphics state current, and resets graphics state.

Deprecated

