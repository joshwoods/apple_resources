

- AppKit
- NSGraphicsContext
-  setGraphicsState(\_:) Deprecated

Type Method

# setGraphicsState(\_:)

Makes the graphics context of the specified graphics state current, and resets graphics state.

macOS 10.0–10.10Deprecated

``` source
class func setGraphicsState(_ gState: Int)
```

Deprecated

This method has no effect

## Discussion

The `graphicState` identifier must be created in the calling thread.

## See Also

### Managing the Graphics State

class func restoreGraphicsState()

Pops a graphics context from the per-thread stack, makes it current, and sends the context a restore graphics state message.

func restoreGraphicsState()

Removes the context’s graphics state from the top of the graphics state stack and makes the next graphics state the current graphics state.

class func saveGraphicsState()

Saves the graphics state of the current graphics context.

func saveGraphicsState()

Saves the current graphics state and creates a new graphics state on the top of the stack.

