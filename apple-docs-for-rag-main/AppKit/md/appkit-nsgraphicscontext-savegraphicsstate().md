

- AppKit
- NSGraphicsContext
-  saveGraphicsState() 

Type Method

# saveGraphicsState()

Saves the graphics state of the current graphics context.

macOS

``` source
class func saveGraphicsState()
```

## Discussion

This method sends the current graphics context a saveGraphicsState() message and pushes the context onto the per-thread stack.

## See Also

### Managing the Graphics State

class func restoreGraphicsState()

Pops a graphics context from the per-thread stack, makes it current, and sends the context a restore graphics state message.

func restoreGraphicsState()

Removes the context’s graphics state from the top of the graphics state stack and makes the next graphics state the current graphics state.

func saveGraphicsState()

Saves the current graphics state and creates a new graphics state on the top of the stack.

class func setGraphicsState(Int)

Makes the graphics context of the specified graphics state current, and resets graphics state.

Deprecated

