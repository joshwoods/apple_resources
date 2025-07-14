

- Core Graphics
- CGContext
-  restoreGState() 

Instance Method

# restoreGState()

Sets the current graphics state to the state most recently saved.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func restoreGState()
```

## Discussion

Core Graphics removes the graphics state at the top of the stack so that the most recently saved state becomes the current graphics state.

## See Also

### Saving and Restoring Graphics State

func saveGState()

Pushes a copy of the current graphics state onto the graphics state stack for the context.

