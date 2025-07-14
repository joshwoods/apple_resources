

- AppKit
- NSPrintOperation
-  destroyContext() 

Instance Method

# destroyContext()

Destroys the print operation’s graphics context.

macOS

``` source
@MainActor
func destroyContext()
```

## Discussion

Do not invoke this method directly—it is invoked at the end of a print operation.

## See Also

### Managing the Drawing Context

var context: NSGraphicsContext?

The graphics context object used for generating output.

func createContext() -> NSGraphicsContext?

Creates the graphics context object used for drawing during the operation.

