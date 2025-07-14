

- AppKit
- NSPrintOperation
-  createContext() 

Instance Method

# createContext()

Creates the graphics context object used for drawing during the operation.

macOS

``` source
@MainActor
func createContext() -> NSGraphicsContext?
```

## Return Value

The graphics context object used for drawing. This object is created using the settings from the receiver’s `NSPrintInfo` object.

## Discussion

Do not invoke this method directly—it is invoked before any output is generated.

## See Also

### Managing the Drawing Context

var context: NSGraphicsContext?

The graphics context object used for generating output.

func destroyContext()

Destroys the print operation’s graphics context.

