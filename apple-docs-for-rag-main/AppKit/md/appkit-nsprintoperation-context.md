

- AppKit
- NSPrintOperation
-  context 

Instance Property

# context

The graphics context object used for generating output.

macOS

``` source
@MainActor
var context: NSGraphicsContext? { get }
```

## Return Value

The graphics context object used for drawing during the operation.

## See Also

### Managing the Drawing Context

func createContext() -> NSGraphicsContext?

Creates the graphics context object used for drawing during the operation.

func destroyContext()

Destroys the print operation’s graphics context.

